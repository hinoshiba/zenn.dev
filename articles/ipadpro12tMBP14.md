---
title: "プログラマな僕が iPadPro 12.9 からMacbookPro 14へ乗り換えた話"
emoji: "🐇"
type: "tech"
topics: ["M1", "iPad", "Macbook"]
published: true
---

こんにちは。hinoshibaです。  
個人の趣味として、休日に欲しいツールのコードを書いています。  
実は、ここ16ヶ月の間ぐらいは、iPad Pro 12.9を活用し開発作業を行なってきました。  
今回、私は、本記事で紹介する問題点によって、Macbook Pro 14 M1 Pro に乗り換えましたが、iPad Pro 12.9 でも十分に開発作業を行えていたので、これから検討される方に向けて、 **iPad Pro関するレビュー記事** を残そうと思います。  
（執筆時点最新の、iPadOS 15.xに対する話なので、iPadOSの将来の更新で挙動が変化する可能性はあるとは思います。）  


# iPad Pro 12.9 での開発は可能

まず、お伝えしたい点としては、iPad Pro 12.9 インチで開発はそこまで困らなかったという点です。（後ほど記事中で触れますが、私がiPad Proをやめたのは、私の使い方が合わなかったというのが大きいと思います。）  
現在のiOSではファイル操作が行いやすくなり、各種エディタのアプリと、Git管理アプリ（[GitHub](https://apps.apple.com/jp/app/github/id1477376905), [Working-Copy](https://apps.apple.com/jp/app/working-copy-git-client/id896694807) 等）の連携がスムーズに行えた印象があります。  

加えて、併売されている、[iPad Pro 12.9 Magic Keyboard](https://www.apple.com/jp/ipad-keyboards/) を用いることで、PCでのコーディングと遜色なく扱うことができました。  

最近ですと、[GitHub Codespace](https://github.com/features/codespaces) など、ブラウザで開発できるサービスも増えてきているので、高レイヤなものであれば、ますます、単体での開発が可能となるとは思います。  

# 利用していた構成

しかし、低レイヤな検証が難しいことや、アプリ境界の都合などで、超えられない壁があることは購入当時からわかっていました。  
それらの領域に関係する作業をしたい場合は、iPad Proの選択は難しいと思われます。  
そのため、一部そのような作業を行いたい私は、アプリの機能を使うことは少なく、以下のような構成で、iPad Proをコンソール機器として利用していました。  

![](/images/articles/ipadpro12tMBP14/overview.png)  

主に、SSHクライアントアプリ（[Blink Shell](https://apps.apple.com/jp/app/blink-shell-mosh-ssh-client/id1156707581) ）と、RDPクライアントアプリ（[Microsoftリモートデスクトップ](https://apps.apple.com/jp/app/microsoft-%E3%83%AA%E3%83%A2%E3%83%BC%E3%83%88-%E3%83%87%E3%82%B9%E3%82%AF%E3%83%88%E3%83%83%E3%83%97/id714464092) ）を活用し、PCのように活用していました。  

## 上記構成の使用感

Blink Shellでは、SSHキーや.ssh/configのような設定ファイルを書くことができ、SSHポートフォワードや、多段SSHのProxyCommand設定も可能です。  
さらに、MagicKeyboardのマウスやキーボードは、とても操作性がよく、SSH作業中は、PCと遜色なく作業ができました。（私は、screen + vim, muttを主環境とするので、本当困りませんでした。）  
Linuxで上げたDockerコンテナ上のHTTPDをポートフォワードし、iPad上で動作確認するといった使い方もでき、動作確認も快適に行えておりました。なお、MagicKeyboardには、ESCキーがありません。SSH環境では、ESCが無いことが課題となるかと思っていましたが、「`Ctrl - [`」に体を矯正できたので、特に問題は感じませんでした。  

ご存じない方が読まれている可能性もあるので、「`Ctrl - [`」のキーコードがESCとなる解説記事を一応貼り付けておきます。  
参考: [tyruさん: 端末アプリで `Ctrl-[` が Esc になる理由](https://tyru.hatenablog.com/entry/2018/10/04/151740)

また、iPad Pro 12.9で動作している iPadOS(やiOS）には、L2TP/IPsec クライアントの機能があります。  
iPad Pro は、Cellular Modelを購入することでSIMが入り、モバイル通信が可能です。  
そのため、VPNサーバ構築とSIMの契約を行うことで、どこでもさっと作業ができる環境を整えることが可能です。  
SIMの刺さらないMacbook と異なり、どこでもさっと開いてSSHやRDP、アプリを用いた簡単なPullRequestの確認など、持ち運ぶ場合の利便性は高く感じました。  

# 不満点

持ち運び開発コンソール用途としてのiPadにはとても満足していましたが、日々の利用から、気になる課題が2つ見えてきました。  

## 1. 言語切り替えUIの出現時間の長さ

「Ctrl - Space」や、「言語切り替えキー」で変更時に出現する以下のUIです。  

![](/images/articles/ipadpro12tMBP14/switch_lang.png)  

このUI、macOSだと「Ctrl」もしくは、「Space」が離された時点で消えてくれますが、**iPadOSでは秒数（体感1秒ちょっと）画面上に残ります**。  
文字列入力は受け付けてくれるため、入力は困りません。しかし、十字キーによる操作がこのUIに持っていかれ、意図せぬ言語切り替えが発生します。  
私は、vimを用いて、日本語のREADME.mdの作成等を行うため、日本語<->English(US) の切り替えが頻繁に発生します。この切り替え直後に十字キーを押すことが割とあったため、意図せぬ切り替えにストレスを感じていました。  

## 2. iOSアプリサスペンドによる、SSHアプリのトンネル停止（suspend）
こちらが、**iPad Pro 12.9での開発をやめた決定的な理由**とも言えます。  
iPadやiPhoneは、電力やリソースの効率化のために、バックグラウンドアプリのサスペンドがあります。（参考：[Managing Your App's Life Cycle](https://developer.apple.com/documentation/uikit/app_and_environment/managing_your_app_s_life_cycle)）  
バックグラウンドアプリは即時サスペンドされるわけではなく、[backgroundTimeRemaining](https://developer.apple.com/documentation/uikit/uiapplication/1623029-backgroundtimeremaining) で取得できる時間ほどでサスペンドされるとのことです。この時間が、非常に短い...。（環境によって異なるらしいですが、概ね20秒から30秒らしいです。）  
そのため、ポートフォワードしたSSHクライアントアプリをバックグラウンド化しているとトンネルがsuspendします。  
利用者の間では割と認知されている話となっており、SSHクライアントアプリの[Termiusがワークアラウンドを提案している記事](https://docs.termius.com/faq/troubleshooting/cant-run-in-the-background) もあったりします。

私はモバイル回線を主に用いていましたが、カフェなどでの作業時は、いわゆるギガ節約のため、カフェのフリーWifiを活用していました。  
フリーWifiを活用するようになって初めて気がついたのですが、割とVPNがうまくいかない環境が多くあります。おそらく、SSTPやOpenVPNですと問題にならないのかと思いますが、iPadOSがbuiltinで扱えるVPNは、L2TP/IPsec であるため、おそらく[NAT Traversal](https://www.infraexpert.com/study/ipsec15.html) が有効でない環境で詰まるようです。  
そのような状況のため、カフェなどのフリーWifiではSSHポートフォワーディングを主に活用していました。  
そして、20秒から30秒で3389(rdp)のポートフォワードが停止するストレスに悩まされる状況でした。  

私はワークアラウンドとして、[SplitView](https://support.apple.com/ja-jp/guide/ipad/ipad08c9970c/15.0/ipados/15.0) や[SlideOver](https://support.apple.com/ja-jp/guide/ipad/ipadfe7c65e9/ipados) による、sshアプリのフォアグラウンド化で乗り切っていましたが、  
使わないターミナルウィンドウが常に画面を占有する状況となり、とてもストレスを感じておりました。  

# MacbookPro 14 の購入まで

iPad Pro購入からの日々、私の利用環境にも変化が現れてきました。  
それは、シェアオフィスの契約です。  
感染症の影響で外に出るべきではないことは承知していますが、私が四六時中家にいる事が妻へのストレスとなるため、あえて外に出る日を作っていました。カフェや公園で作業をする事も多々ありましたが、作業場所を探す手間やドリンク代のコストよりシェアオフィスの特定プランが安いと思われたため、9月よりシェアオフィスの契約を行いました。（土日祝日プランで個人用途）  

これにより、フリーWifiの安定供給が見込まれ、コンソール端末がモバイル回線を扱える事の重要性が薄まりました。  
iPad Proを選定した理由の大半を占めているのが、モバイル回線の利用でした。そのため、フリーWifiの安定供給が見込まれると、コンソール用途の端末がiPad Proである必要性がなくなってきます。  

そして、タイミングよく、[2021/10/18(現地時間) にM1Pro/Max シリーズが搭載されたMacbook Proが発表](https://www.apple.com/jp/newsroom/2021/10/apple-unveils-game-changing-macbook-pro/)されました。  
私はもともと、クロスコンパイルのarm動作確認用やゲームのために、M1 Mac miniを所有していましたが、こちらは一部性能不足を感じる事がありました。  
そのため、iPad Pro 12.9 と、M1 Mac miniのリプレースとして、Macbook Pro 14 M1 Proの購入を決めました。  

# iPad Pro 12.9 も使い勝手は良かった

本記事は、購入したMacbook Pro 14の使用感を試すためにタイピングすべく作成してみました。  
ここまでタイピングした感覚や参照情報を漁った感覚、使いづらさは感じません。また、画面のミニLEDディスプレイは目の疲れづらさが少ないように感じます。  

とはいえ、iPad Proから劇的に使いやすくなったか。と問われると、上げた不満点2つ以外、私の使い方上の改善点は特に感じません。（iPad Proも今はミニLEDですし。）  
むしろ、たまにApple Pencil 2にて概要図等をまとめていたため、これからどうしようと悩む方事すらあります。  

私の使い方では、重要なポイントでマッチしない点があり、iPad Proによる開発を諦めましたが、それらを除けば開発用途で問題がありませんでした。  
MagicKeyboardやApple Pencil2を揃えていくと20万円越えではありますが、フットワークの軽さはPCを超えるものがありました。  

端末の検討は難しく試行錯誤しておりますが、iPad Pro も開発端末として優秀であることは確かです。  
検討されている方いらっしゃいましたら、ぜひ参考にください。  
