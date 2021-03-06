---
title: "作業環境をDockerfileにまとめて、macOSでもLinuxでもWSL2でも快適に過ごせるようになった話"
emoji: "🐇"
type: "tech"
topics: ["Docker", "Linux", "macOS", "WSL", "作業環境", "環境"]
published: true
---


こんにちは、CLI生活至上主義？の、 ひのしば です。  
まぁ、至上主義というのは、ちょっと言い過ぎかもしれませんが、screen, vim, mutt, newsboat, pass, あとは、gitやssh 辺りを使う生活をしており、1日の作業がこれだけで完結するような事もあるような生活を送っています。  

さて、そんな私が、ワークステーションサーバに、macOSや、Windows, Linuxから接続して操作するといった構成から、  
作業環境をDockerfileにまとめ、手元で上がる環境をdockerコンテナへ統一し作業する構成とした話を紹介します。  

この環境は、ここ数ヶ月、不自由なく使えている事もあり、自身の整理のためにも、どのような点が気になって対応したのかを挙げていきます。  
詳細は下部に記載する通りですが、  
例えば、dockerfile上のuidの問題に気をつける点、LinuxとmacOSのユーザフォルダPATHの違いを気をつけた点、docker outside of dockerを扱えるようにした点などがあります。  

# これまでの環境
[過去に記事でも紹介](https://zenn.dev/hinoshiba/articles/ipadpro12-mbp14#%E5%88%A9%E7%94%A8%E3%81%97%E3%81%A6%E3%81%84%E3%81%9F%E6%A7%8B%E6%88%90)したことがありますが、私の作業環境は以下のような構成となっておりました。  

![](/images/articles/ipadpro12-mbp14/overview.png)  
(画像の接続元は、iPadProとなっておりますが、他にもmacOSやWindowsなどをコンソールとして用いていたイメージです。)  

基本的にCLIな作業は全てworkstation上のプロセスとして動作させ、それらをいじるためのscreenセッションを1つ起動しておき、各クライアントによるsshからscreenにattachする生活をしておりました。  
正直いいますと、私の用途では、macOSやWindowsが手元にある状況では、あえてLinuxへattachする必要性は、ありません。  
しかし、環境差異がどうしても気になり、このような構成を取っておりました。  
具体例をあげると、  
* 同じようなCLIツールを入れるにしても、パッケージマネージャ(brew, aptなど) の違いがある
* アーキテクチャ、OSの違いにより、依存物等が違う/そもそもインストールできない
* デフォルトのshellが違う(zsh, bash, ...)
* コマンドのデフォルト引数や、挙動が微妙に違う

などです。  

設定の変更でどうにかなる点もありますが、そもそも設定を頑張る事自体が苦でした。  
であれば、最初から一つの環境に集中し、そこを異なる環境から扱うようにしようと考えたわけです。  

# これまでの環境における課題

1つの環境に集中したとしても、管理するものは少なからずありました。  
`.gitconfig`のような設定ファイル(dotfile)群です。  

みなさんは、どのように管理されていますかね。  

私は、`/home/<myuser>` 配下をgit化し、remote repositoryに上げて、バックアップ兼構成管理としていました。  
しかし、この方法、インストールしているソフトウェアのバージョンは一緒に管理されていません。  
そのため、ソフトウェアの入れ直しや、作業環境環境の引っ越しなどで、そのまま動作しないといったストレスを抱えておりました。  
作業環境DRにて扱うケースや、職場で私用の`.vimrc`を参照したいケースでもうまく行かないケース も稀にあり、その度に環境毎で分岐しそうになる自身のdotfileに頭を悩ませていました。  

上記で挙げた、dotfileとインストールされたソフトウェアをまとめて管理できていないような問題の他にも、  

* `pip`や`gem`、`npm`等にて、意図せずグローバルインストールしてしまったケースへの削除対応ストレス
	* 何かが残っていた際に、たまたまうまくいく(or うまくいかない) ケースへのトラブル対応ストレス
* ネットワーク越しに環境を利用するので、高レイテンシ下での、入力から反映までのレスポンス遅延によるストレス

を感じておりました。  
今回紹介するdockerfileに移行する直前ぐらいまでは、`pip`などを扱う際には、LXCを用い、まずは環境分離をすることから始めていましたが、  
直前までの編集環境との差異が生まれ、少しインストールコストがかさむなともやもやした日々を過ごしていました。  

# 欲しいのは、同じように扱える環境

2021年の年末、（ちゃんと計測したわけでは無いのでおそらく）docomoの電波の境目と思われるカフェで作業する機会がありました。  
とにかくインターネット接続が安定しません。過去の私の構成では、インターネット接続が安定しないとVPNが接続できず、作業環境に接続することができないのです。  
その際に、久しぶりに泣く泣くオフライン作業をしたのですが、やはり効率が下がります。というか、効率が下がりすぎ作業にならないことからどうにか環境を変えられないか考えておりました。  

また、その頃は、2022年頭での転職を考えており、次の職場での環境構築もめんどくさいだろうなと考えており、  

持ち運びしやすい共通な環境は作れないだろうか。と思案するきっかけとなりました。  

# dockerfileで管理すればいいのではないか。

設定ファイルとソフトウェアの環境をまとめて管理するという観点だけでは、例えば、Ansibleなどでも問題がありません。  
しかし、本記事の最初でも語っている通り、環境差異によるストレスもどうにかしたいという思いがあります。  

そこで、設定ファイルとソフトウェアをコーダブル管理でき、あわよくばアーキテクチャも明示指定した起動が可能な、共通のコンテナ自体を日々の作業環境として利用することを考えました。  
色々な検討の結果、共通インタフェースとしては流行りのdockerfileを採用する事としました。  

# 私のDockerfile'sな作業環境
さて、ようやく Dockerfile環境の紹介です。  

まず、リポジトリは以下に保管しています。  
https://github.com/hinoshiba/dockerfiles  

とても雑に簡単に紹介すると、`make target=workbench` とすれば作業環境を使えるように準備しています。  
dockerへの引数は、毎回同じようなものを指定することも多いので、それらはmakefileにまとめてしまい、  
`target=<target name>` といった指定で、`リポジトリroot/dockerfiles/<target name>/Dockerfile` を対象として呼び出せるような構成にしています。  

ちなみに、`target=workbench`は、私の普段の作業用コンテナです。ファイルとしては、以下を起動します。  
[github.com/hinoshiba/dockerfiles/dockerfiles/workbench/Dockerfile](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/dockerfiles/workbench/Dockerfile)  

上記ファイルのFROMにある通り、base イメージは、ubuntuを用いています。  
本イメージに、aptでインストールするソフトウェア一覧をdockerfile上に一緒にまとめ、同一リポジトリの以下に、設定ファイルを格納しています。  
[github.com/hinoshiba/dockerfiles/dockerfiles/workbench/dotfiles/](https://github.com/hinoshiba/dockerfiles/tree/73efd001cea6d4998121944db52ad0af9431543b/dockerfiles/workbench/dotfiles)  

これにより、macOSでも、Linuxワークステーションでも、Windows(WSL2) でも、使い勝手が統一されたubuntuなCLI環境を扱うことを実現しています。  

ちなみに、イメージの更新は、一度実行コンテナを停止(`make stop target=workbench`)し、再ビルド(`make build target=workbench`)すれば良いフローにしています。  
変更がある場合も、git logで追いかけやすく、`apt dist-upgrade`もdokcerイメージ再ビルドで走るので、考える事が無くなりました。  

# 本環境を作るに辺り検討した点

さて、[Makefile](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/Makefile) をみていただくとわかるのですが、オプションの生成を色々と頑張っています。  
いくらdockerが共通インタフェースを提供しており、Dockerfileで簡単に扱うことができるものとはいえ、私の使い方では、いくつかの歯痒いところがあったので、それらをMakefileや各種スクリプトで支援しています。  
具体的に5つだけ紹介します。  

## 1. secretファイル等の扱い
いくら統一的な環境とはいえ、`.gnupg`や`.ssh`のようなシークレットファイルとすべきようなものを共通利用をすることは気が引けます。  
他にも、`.gitconfig`や、`.muttrc`のようなある程度動作環境事に使い分けたいものもあります。  

これらについては、複数の環境でまとめて扱うことが難しいので、以下のようにmount対象とすることで、ホスト上に存在するファイルをそのまま利用しています。  
```Makefile
		useropt+= --mount type=bind,src=$(HOME)/.ssh,dst=$(HOME)/.ssh,ro
		useropt+= --mount type=bind,src=$(HOME)/.ssh/known_hosts,dst=$(HOME)/.ssh/known_hosts
		useropt+= --mount type=bind,src=$(HOME)/.gnupg/openpgp-revocs.d,dst=$(HOME)/.gnupg/openpgp-revocs.d,ro
		useropt+= --mount type=bind,src=$(HOME)/.gnupg/private-keys-v1.d,dst=$(HOME)/.gnupg/private-keys-v1.d,ro
		useropt+= --mount type=bind,src=$(HOME)/.gnupg/pubring.kbx,dst=$(HOME)/.gnupg/pubring.kbx,ro
		useropt+= --mount type=bind,src=$(HOME)/.gnupg/pubring.kbx~,dst=$(HOME)/.gnupg/pubring.kbx~,ro
		useropt+= --mount type=bind,src=$(HOME)/.gnupg/trustdb.gpg,dst=$(HOME)/.gnupg/trustdb.gpg,ro
		useropt+= --mount type=bind,src=$(HOME)/.gitconfig,dst=$(HOME)/.gitconfig,ro
		useropt+= --mount type=bind,src=$(HOME)/.muttrc.add,dst=$(HOME)/.muttrc.add,ro
		useropt+= --mount type=bind,src=$(HOME)/.muttrc.signature,dst=$(HOME)/.muttrc.signature,ro
		useropt+= --mount type=bind,src=$(HOME)/.muttrc.passwords.gpg,dst=$(HOME)/.muttrc.passwords.gpg,ro
...#省略
	$(D) run --name $(NAME) -it $(useropt) $(rm) $(mt) $(portopt) $(dopt) $(builder)/$(TGT) $(INIT_SHELL)
```
[上記例が含まれるMakefileへのリンク](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/Makefile#L52)  

合わせて、以下のような手順を作成し、利用前の準備として作成する運用をしています。  
https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/docs/workbench/setup.md  

## 2. 起動と接続は考えなくて良い
作業をする度に、起動させて接続する(`docker run`)か、起動済みの環境に接続する(`docker exec`)かを使い分けるのは少し手間です。  
そのため、`make target=workbench`と入力すると、workbenchが起動していれば起動しているコンテナへ。起動していない場合は起動させてから接続する。といった工夫をしています。  
もちろん、2コンテナを使い分けたいケースも考え、`make target=workbench cname=wb-container02` のように、cnameといったオプションでコンテナ名を指定でき、複数選択も実現しています。  

## 3. 残すべきファイル群
コンテナは、継続的に残すべきといったポリシーではなく、一時的な検証で何かを追加し汚れたらコンテナを上げ直せばいいといったポリシーで考えています。  
先ほどあげた`pip`などで間違えてグローバルインストールした際などが該当します。  
恒久的に欲しいと思ったものは、Dockerfileに追加すれば良いですし、`pip`で追加したものが一時的なもので恒久的に不要であれば、コンテナを上げ直せば元に戻ります。  

しかし、それらの観点とは別に、「残しておきたい、作業中のファイルやhistoryファイル」や、「残しておくと処理が楽になる、cacheファイル」等があります。  

これらについては、`.shared_cache`や`~/git`、`work`といったファイルを[ホストと共有するといったオプションを用意するようにMakefileへ記述](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/Makefile#L43) しており、コンテナを削除してもファイルが残るようにしています。  
このコンテナの用途は、共通の作業環境が欲しいのであり、ホスト自体のデータとしてのファイルをいじることは問題ではないので、このようにしています。  

おかげで、コンテナを再起動しても、`ctrl + r`にて、`reverse-i-sseach`を起動し、先ほどのコマンドを利用することも可能です。  
コンテナを止め、イメージを上げ直しても先ほどまでのhistoryが引き継がれるので、コンテナを削除する心理的ハードルも下がっています。  

## 4. コンテナエンジンホストと、コンテナ上での同一UIDの利用
LXCと異なり、Dockerは何も考えないとコンテナ内部のユーザはrootで起動します。  
また、Linux上(と、WSL2上)のDockerは、コンテナにマウントして作成したファイルは、何も考えないとuid=0として扱われてしまいます。(macOSは、挙動が異なります。)  

この問題では、`docker run`時に、`-u <uid>:<gid>` オプションを指定するといった方法をよく見かけます。  
しかし、この方法ですと、userを作成しているわけでは無いので、homeフォルダが存在しないといった状況が生まれてしまいます。  
少しの検証であれば、これは大きな問題では無いのですが、dotfileやcacheを、環境変数`${HOME}`など利用したいようなソフトウェアでは、homeフォルダが存在しない事が問題となります。  

このため、コンテナ起動時にユーザを作成すると言った方法を行っています。  
具体的には、[exec_users.sh](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/dockerfiles/workbench/exec_user.sh) というスクリプトを用意しており、以下の工程でユーザを作成しています。  

1. 呼び出し元Makefileにて、makeファイルを呼び出したUID, GID, Username等を解決
2. docker runの環境変数に、UID, GID, Username等を含めることで、本スクリプトが受け取り、ユーザがいない場合、一致するユーザを作成する
	```bash
	USER_ID=${LOCAL_UID:-9001}
	GROUP_ID=${LOCAL_GID:-9001}

	getent passwd ${LOCAL_WHOAMI} > /dev/null && exec_usershell

	echo "Starting with UID : $USER_ID, GID: $GROUP_ID"
	useradd -u $USER_ID -o -m ${LOCAL_WHOAMI}
	groupmod -g $GROUP_ID ${LOCAL_WHOAMI}
	passwd -d ${LOCAL_WHOAMI}
	usermod -L ${LOCAL_WHOAMI}
	```
3. sudo等の必要なグループへの追加
	```bash
	gpasswd -a ${LOCAL_WHOAMI} docker
	...
	echo "${LOCAL_WHOAMI} ALL=NOPASSWD: ALL" | sudo EDITOR='tee -a' visudo
	```
4. キャッシュファイル、設定ファイルのコピーや生成
	```bash
	chown -R ${LOCAL_WHOAMI}:${LOCAL_WHOAMI} /etc/dotfiles
	...
	sudo -u ${LOCAL_WHOAMI} cp /etc/dotfiles/bashrc /home/${LOCAL_WHOAMI}/.bashrc
	# 等の続く処理...
	```
5. 作成したユーザにて、/bin/bashを呼び出すsudoを、execする
	```bash
	cd "${LOCAL_HOME}"
	exec sudo -u ${LOCAL_WHOAMI} /bin/bash
	```

作成中に、sudoへの追加も行っているので、一般ユーザを作成したとしてもsudoによって後からコンテナに何か特権変更を加える事も可能としています。  
ごく稀に何か足りなかった際に、`apt install`などができるため、重宝します。  
もちろん、恒久化するには、試した後に、Dockerfileへ加筆することを忘れないようにしなくてはいけません。  

ちなみに、docker image生成時にアカウントを作成する方法もあります。  
しかし、その場合、imageにローカルアカウント名が保管されてしまいます。  
もし将来、dockerhubなどでイメージを上げたくなった際に、セキュリティ的な懸念事項となる事が考えられました。  
そのため、dockerコンテナの最初の処理として、ユーザを作成しています。  

## 5. docker outside of dockerをストレスなく使える

docker outside of docker自体の説明は割愛しますが、  
簡単に説明すると、dockerのsocketファイルをコンテナ内部に共有することによって、コンテナ内部から、コンテナエンジンのdockerに命令を出せるものです。  
コンテナ内部から命令を出すのは、特に難しいものではなく、[Makefileのここ](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/Makefile#L60) でやっているように、`/var/run/docker.sock` をmount対象に追加するだけです。  
```Makefile
useropt+= --mount type=bind,src=/var/run/docker.sock,dst=/var/run/docker.sock
```

しかし、特に何も考えずにコンテナから命令を出すと少し悩ましい事が起きます。リソース周りの問題です。  
リモートのコンテナエンジンを利用している時と少し近いのですが、docker outside of dockerのコンテナエンジンが参照するリソース（通信、ファイル等）は、コンテナ内部ではなく、コンテナエンジン側のリソースを扱います。  
そのため、例えば、作業用コンテナ内部に`/home/<user>/hoge/Dockerfile` といったファイルを作成しても、コンテナエンジン側にはそのようなファイルが存在しないため、`docker build /home/<user>/hoge/Dockerfile` は、失敗するといった状況が生まれます。  

これらを解決するために、実行ユーザ名を揃え、共通のPATHとなるようにマウントする方法を取っています。  
お察しかもしれませんが、既に紹介した、`4. コンテナエンジンホストと、コンテナ上での同一UIDの利用` と、`3. 残すべきファイル群` が、本項目の解決もしています。  
ちなみに、実は、`4. コンテナエンジンホストと、コンテナ上での同一UIDの利用` にて、`Username` を揃える事を紹介していますが、4の目的では、`Username`を揃える必要がありません。  
コンテナエンジンであるホストと、コンテナのPATHを一致させたいために、あえて`Username`を一致させています。  
このような構成にすることで、dockerコマンドを作業用コンテナから実行したい場合は、`3. 残すべきファイル群` にて紹介した、`work`や`git`上に、Dockerfileを設置すると、  
コンテナ内部とコンテナエンジンに存在するファイルとPATHが揃い、コンテナ内部で入力したPATHがそのまま利用できます。  

### macOSは、`/Users/<user>` なので。
Ubuntuのデフォルトのユーザホームは、`/home/<user>`ですが、macOSでは、`/Users/<user>`です。  
これらの差分もスクリプト側などで吸収しきれないと、統一的な利用ができる環境ではなくなってしまいます。  

これを解決するために、exec_user.shにてユーザを作成する際に、任意のHOMEを指定しています。  
```bash
test "${LOCAL_HOME}" == "/home/${LOCAL_WHOAMI}" || (rm -rf "/home/${LOCAL_WHOAMI}" && ln -s "${LOCAL_HOME}" "/home/${LOCAL_WHOAMI}" && usermod -d "${LOCAL_HOME}" "${LOCAL_WHOAMI}")
```
[上記のexec_user.shの該当箇所リンク](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/dockerfiles/workbench/exec_user.sh#L28)  

動作としては、[Makefileで環境変数LOCAL_HOMEを解決](https://github.com/hinoshiba/dockerfiles/blob/73efd001cea6d4998121944db52ad0af9431543b/Makefile#L36) し、`/home/<user>`ではないパターンだったらシンボリックリンクの作成と、ユーザのHomeを切り替えています。  

これにより、`/Users/<user>`であっても、`/home/<user>`であっても、`/rabbit-love/<usre>`だったとしても統一的な利用が可能です。  


# macOSでもLinuxでもWSL2でも快適に過ごせるようになった

さて、このように、いくつかの工夫により、コンテナ上の作業環境を、気軽に再構築しつつ、データを保持でき、  
OSが異なる環境でも統一的なインタフェースで扱うことを実現できました。  

扱う環境がUbuntuベースでそろってもいるので、「コマンドのインストール方法やオプションが違う」「挙動が微妙に異なる」といった悩みからも一旦解放され、  
「環境自体の再構築も低コスト」に、「何か試したい場合にコンテナを汚しても即時リセットができ」、「環境のコーダブルな差分管理もできている」といった、私としては嬉しい事三昧の環境が完成しました。  

また、環境には、dockerが入っていればいいので、do-release-upgradeにドキドキする事も無くなりました。(新しく環境を作りたければ、dockerを入れて、秘密なファイル群を再生成すれば済みます。)  
トレーニングの仮想環境にて、自身の環境を構築しなくてはいけないケースや、仕事で扱う環境を構築しなくてはいけないケースであっても、docker入れて秘密系なファイルを作成するだけなので、そのような状況においても恩恵があったなと感じています。  

---

さて、いかがでしたでしょうか。

このような形に構築できたことで、日々の環境保全の悩みはここ数ヶ月、起きていません。  
今後よりよい環境保全の方法が思いつけば、移行する事はあるでしょうが、しばらくはこのままかと思っています。  

なお、紹介できていない工夫は他にもありますが、そちらについては、リポジトリをぜひ覗いて見てもらえればと思います。  
ちなみに私はdockerプロではないので、懸念点がありこうした方がいいのではないか？と言ったお話があれば、PRなり、コメントなりありましたらぜひ、お待ちしております。  
(また、本方法以外で環境を保全されているよりよい方法などありましたら興味があるので知りたいところです。)  

# 補足

今回は、私の作業環境である`target=workbench`に焦点を当てて紹介しました。  
他にも`target=golang`と行った形で、普段の作業環境を https://github.com/hinoshiba/dockerfiles/tree/master/dockerfiles にまとめています。  
workbench以外では、ユーザ環境とPATHを揃える必要が無いので、そのような準備は特にしてませんが、dockerコマンドを意識しなくても扱える辺りは一緒です。  
また、今回紹介はしていませんが、[用意しているMakefile](https://github.com/hinoshiba/dockerfiles/blob/master/Makefile) では、他のオプションも用意しており、  
コンテナへのportマッピングやrootでの起動、任意のファイルのマウントもmakeから簡単に指定できるようにしており、dockerコマンドを意識することなく扱える構造にしています。  
オプションの説明は、[こちら](https://github.com/hinoshiba/dockerfiles/blob/master/docs/options.md) にまとめています。  
