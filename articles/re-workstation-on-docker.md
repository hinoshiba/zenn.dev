---
title: "作業環境をDockerfileにまとめて、快適に過ごせるようになった、その後"
emoji: "🐇"
type: "tech"
topics: ["Docker", "Linux", "macOS", "WSL", "作業環境", "環境"]
published: true
---

こんにちは、ひのしば です。  

会社と個人のvimrcファイルの乖離や、BSD系のsedに苦しめられることが無いよう、macでもWindowsでも快適なターミナル生活を送るために、[作業環境をdockerfile群](https://github.com/hinoshiba/dockerfiles) としてまとめています。  
本環境については、2年ほど前に [作業環境をDockerfileにまとめて、macOSでもLinuxでもWSL2でも快適に過ごせるようになった話](https://zenn.dev/hinoshiba/articles/workstation-on-docker) という記事をzenn上にあげました。私個人のブログとしては、割と多くの反応をいただき、かなり記憶に残っています。  

この記事の投稿以降も、自身の作業環境に対するメンテナンスとして、気になる点の更新を行い続け、かなり理想郷へ近づいてきていると感じています。  
具体的な変化は、[以前のブログと現時点のHEADのdiff](https://github.com/hinoshiba/dockerfiles/compare/73efd001cea6d4998121944db52ad0af9431543b...16ca1a3f0a6acf6d05ace141c358315f5a0ed136) を見ることで確認ができますが、  
コードベースだと私のこだわりの変化をお伝え仕切れないかもしれないので、いくつかポイントを紹介します。  

# バージョンをよしなに更新して欲しいが、更新があることは気がつきたい。あと、メジャーバージョンアップは、手動でハンドルしたい

各dockerfileの中には、`apt-get update && apt-get dist-upgrade -y` のような事を行うため、各ディストリビューションや言語パッケージ側に最新のバージョンがある場合、イメージの再buildを行えば、最新の状態に更新することが可能でした。  
ただし、元となるイメージ自体のタグについては、手動更新せざるを得ず、そのタグに対するバージョン確認が手動タスクとして残ることが悩みでした。  
`FROM <software>:latest` のような指定を行い、ハンドリングをやめてしまっても、問題はありませんが、マイナーバージョンアップに限っては、skipしたいケースや戻したいケースも考えられるため、更新に気がつきつつ、更新可否を指定できるような運用を検討しました。  

## バージョン修正箇所を集約した
バージョン管理を行うにあたり、バージョン記載場所が複数箇所に点在することへの解決を第一に考えました。  
複数箇所で同一ソフトウェアに対するバージョンを管理すると、一方の更新漏れの可能性があるためです。  
もちろん、明示的に指定したいケースは例外ですが、そのような場合を除き、原則集中管理したいと考えました。  

様々な用途を想定し、本リポジトリ外から参照したいケースの拡張性も考え、バージョン情報を記載した1ファイルを設置する案に至りました。  
例えば、[version/golang](https://github.com/hinoshiba/dockerfiles/tree/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/version/golang) のように、メジャーバージョンと厳格なバージョン指定を行うファイルを設置しています。  

本リポジトリは、GitHub上で管理しているため、[Raw指定でバージョン情報のみを取得](https://raw.githubusercontent.com/hinoshiba/dockerfiles/master/version/golang/major) が可能となります。  
リポジトリ内外いずれも、本PATH等を指定することで、現在私が示したいバージョンを取得することが可能となりました。  

利用方法としては、build-argsやcurlによるコマンド置換を用い、上記ファイルの内容を利用します。  
* `build-args`のパラメータとして、`strict` の値を渡す
    * [dockerfiles/golang/Dockerfile#L2](https://github.com/hinoshiba/dockerfiles/blob/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/dockerfiles/golang/Dockerfile#L2)
* curlによるコマンド置換で値を渡す
    * [dockerfiles/workbench/Dockerfile#L16](https://github.com/hinoshiba/dockerfiles/blob/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/dockerfiles/workbench/Dockerfile#L16)

いずれかの方法を用いることで、私が利用したい主なバージョンを集中管理場所から取得できる形とできました。  
なお、現在管理対象としているものは、[version](https://github.com/hinoshiba/dockerfiles/tree/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/version) というPATH配下にまとめています。  

## バージョンを自動的に確認
バージョン記載場所を集約したことにより、バージョン記載ファイルと最新バージョンを比較し、更新を促すことが可能となりました。  

具体的には、  
マイナーアップデートのPR自動生成( [\[NewVersion\] golang/1.21.12 ](https://github.com/hinoshiba/dockerfiles/pull/157) ) や、  
メジャーバージョンアップのEOL通知Issue ( [golang/1.20 is EOL.](https://github.com/hinoshiba/dockerfiles/issues/119) )   
が、自動で実施されます。  

仕組みとしては、非常に単純であり、`https://endoflife.date/` のAPIを利用し、[バージョン確認のactionsを作成](https://github.com/hinoshiba/dockerfiles/blob/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/.github/workflows/life_pr.yml) しています。  

最も適切なのは、各ソフトウェアのリリースページ自体を確認することだとは考えますが、  
個別パーサの管理を行うことは非常に手間です。  
数時間以内の更新を徹底的に追いかける要件も無いため、大変便利な`https://endoflife.date/` を利用するに至っています。  

## 環境のautoupdate=yes
これまで紹介したバージョン集約やバージョン自動確認に加え、docker imageの生成をGitHub Actionsへ引っ越しをしています。  
2年前の時点では、ローカルにてbuildを行っていましたが、上記2つのアップデートにより、GitHubリポジトリとしてのbuildが非常に有効となりました。  

なんせ、自動生成されたPullRequestをマージすると、対象ソフトウェアが全て更新されるのです。  

また、上記以外にも`apt-get update && apt-get dist-upgrade -y` のような更新を行うケースもあります。  
そのため、週に一度は環境を更新できるよう[docker image buildを行うActionsのcronも設定](https://github.com/hinoshiba/dockerfiles/blob/16ca1a3f0a6acf6d05ace141c358315f5a0ed136/.github/workflows/builder.yml#L4) しています。  

# 運用体験について
今回紹介したバージョン管理方法以外にも、[gitのbranch名をterminalへ表示するように更新](https://github.com/hinoshiba/dockerfiles/pull/143/files) や、[screenのレイアウトを指定する更新](https://github.com/hinoshiba/dockerfiles/commit/8ee0f09ae0b610594ace888579d3e090740e1ce8) 等も行い、2年間、少しずつ便利にしてきました。  
dotfile単体を管理したとしても、実行ソフトウェアのバージョンにより利用方法が異なるオプションもあるため、それらをまとめて管理でき、IssueやPullRequest形式にて、管理できるものは大変取り回しが良いように感じます。  

某海賊漫画のように、覇気を扱えるほど、2年間でアップデートができたかわかりませんが、
ひとつなぎの便利なターミナル生活まで、あと少しのように感じます。  
なお、この2年間で、906行の追加。282行の削除が行われたようです。  
ちょっと冗長な点もありそうなので、もう少しスリムにしていきたいですね...。  
