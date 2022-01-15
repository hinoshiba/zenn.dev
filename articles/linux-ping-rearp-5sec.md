---
title: "LinuxにPingしたら5秒後にARP Requestされる件"
emoji: "🐇"
type: "tech"
topics: ["Linux", "ARP", "Windows", "Network"]
published: true
---

本記事は、2019年頃にQiitaに投稿しましたが、Qiitaを解約したので移動した記事です。  
zennの方が技術者が集まるので、コメントがもらえればと転機します。  
上記理由により、zennの投稿日と実際の記事作成日に乖離があります。  

---

# 前書き
## 記事の目的
* 調べた背景となった事象は説明できるのだけど、
	* Neighbor Cache Entry Statusを将来わすれそうなので遷移をメモ
		* 初心者に優しい感じで日本語/英語共にまとまっている記事がほぼない
	* 半分ぐらい認識しただから間違えていたら詳しい人からツッコミを受けたいので晒す
	* 下述:疑問が残っている点 が知りたいから詳しい人からツッコミを受けたい

# 本題
## 背景
* 仕事中に後輩くんから以下の質問を受け回答できなかったので週末調べて検証した
	* ICMPのtcpdumpを見て勉強しているが受信ホストがWindowsとLinuxの場合で動作が異なる
	* 異なる動作は、LinuxはICMPを受けた場合、5秒後にARP Requestを発砲する。Windowsはそのような動きをしない
	* ARP Request受信時に受信側のARP CacheにARP Request発砲側が登録される想定だが、なぜLinuxは5秒後に再確認をおこなうのか？
* なお、後輩くんの勉強スコープとしては意図しない事象

## 結論
* ARP Request受信時のARP Cache登録は確かに行われるが、ARP Cache登録時のStatusは、自身が次にフレームを送出した一定時間後に再確認を行うであるため、5秒後にARP Requestが発砲される
	* TCPは例外。今回はICMPだったため事象が発生した
* Windowsは純粋なARP Requestのみである場合、同様のStatusでARP Cacheに登録されるが、IPレイヤプロトコルが一定時間内に発生した場合、動作が異なると思われる

## 事象説明への前提認識 : Neighbor Cache Entry Statusについて
* ARP Cache(Neighbor Cache Entry) には、登録されているレコード(IPアドレス対MACアドレス) 毎にStatusが存在する
	* Status毎に動作を変えることで、Cacheを適切な状態。古いものの更新削除を行なっている
* 遷移として覚えておくと良いポイント
	* 通常のTCP通信の場合、連続的に通信を行わない場合でも、[Reachable] -> [Stale] -> [Delay] -> [Reachable] を繰り返す
	* フレームを送出している限り[Reachable]が続く

###  ステータス遷移
![nd_flow01.jpg](/images/articles/nd_flow01.jpg)

### ステータスの詳細説明
|Status名|説明|
|--:|:--|
|None|Cacheへエントリされた状態で、ARP解決前。<br>ARP Request発砲前。|
|Incomplete|ARP解決を行なっている状態。<br>ARP Request後、ARP Reply受信前。|
|Reachable|ARP解決が行えた状態。<br>ARP Replyを受信した。|
|Stale|最後にFrameを送出してから、Reachableの有効期限(Reachable_time)が過ぎた状態。<br>第三者からARP Requestを受信した場合は、本ステータスとなる。|
|Delay|Stale状態のMACアドレスに対して、1つ目のフレームを送出した直後に遷移する。<br>本状態期間中にTCPのACK付き通信を受信した場合、Reachableへ遷移する。|
|Probe|Delayの有効期間(delay_probe_time:デフォルト5秒)を過ぎた状態。ARP Requestを発砲し、解決を試みる。|
|Failed|ARP解決が行えなかった状態。ARP Replyが受信できなかった。|

## 受信側のLinuxで発生していた事象
* ICMP受信側のフローは以下の通りになり、[Delay]で5秒待ち、[Probe]でARP Requestを送出していた
* RFC的には何もおかしくない

![nd_flow02.jpg](/images/articles/nd_flow02.jpg)

1. ICMP送信側ホストは、MACアドレス解決のため、ARP Requestを実施
2. ICMP受信側ホストは、ARP Requestを受信したため、StaleでICMP送信側ホストを登録し、ARP Replyを送出
3. ICMP送信側ホストは、ARP Replyを受信し、ICMPをICMP受信側ホストに向けて送出
4. ICMP受信側ホストは、ICMPを受信し、ICMPを応答する。応答する際にFrameがICMP送信側ホスト向けに送出される為、StaleがDelayへ移る
5. ICMPはTCPのACKを検出できないので、delay_probe_time:デフォルト5秒を超過し、Probeとなり、ARP RequestをICMP送信側ホストに向けて送出する

## Windowsでおきなかった理由
* 正しい説明が見つけられなかったので、検証と動作からの推定です

### Windowsの動作が不明だった為、以下の通り検証をおこなった
* WindowsにICMPを送信した場合、Reachableとなった
* ARP Requestのみをarpingで送りつけた際にはStaleとなった
* Stale時の動作はLinuxと一緒だった
	* WindowsでStale時にICMPを受信させた場合、Probeとなり5秒後にARP RequestがICMP送信側ホストに対して送出された
		* `netsh interface ipv4 show neighbors`では、Delay表現が見れなかったけど、これは写していないだけだと思われる
	* TCP通信の場合、Probeとならず、Reachableとなった

### 検証結果からみられる動き
* おそらくWindowsはARP Request受信時に一定期間待ってからStaleでARP Cacheに登録する動きが想定できる。一定期間待つ時間(まぁDelayStaleとでも呼べる状態でもがあるのかな?)中にIPレイヤ通信が発生した場合、Reachableになる動きをした
	* この動作はLinuxでは見られなかった
	* 第三者情報も多かったが、ARP Cahce話で調査中にWindows Vista以降。という文言をよく見たので、Windows Vistaよりも前だと動作が異なるのかもしれない

#### Windowsの遷移図(推定)
![nd_flow_windows.jpg](/images/articles/nd_flow_windows.jpg)

# 総括
* Linuxホストに対して、ICMPを送出する場合、最初のARP Requestにより、ARP Cacheが[Stale]->[Delay]->[Probe]に遷移し、5秒後にARP Requestを発砲する
* WindowsはDelayStale?があるので、ICMPでは動作が異なり、[Reachable]になっていたため、ICMPを送り続ける間は、ARP Requestが発砲せず、Linuxホストと動作がことなった

# 疑問が残っている点
* delay_probe_timeが5秒な理由
	* /proc/sys/net/ipv4/neigh/default/辺りで変えられるという情報は見るけど、なぜ5秒なのかがどこにも情報ない
	* gc_thresh1の間隔とかも全部default値が5秒な理由が知りたい
* Windowsの動作でDelayStaleと呼んでいる部分の説明がほしい
	* StaleDelayのようなものが本当はどのように存在するのか知りたいけど調べきれていない

# 参考
* https://tools.ietf.org/html/rfc4861#section-7.3.2
* https://wiki.bit-hive.com/linuxkernelmemo/pg/アドレス解決プロトコル
* https://docs.microsoft.com/en-us/windows/desktop/api/nldef/ne-nldef-nl_neighbor_state
* https://linuxjm.osdn.jp/html/LDP_man-pages/man7/arp.7.html

