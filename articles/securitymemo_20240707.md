---
title: "2024/07/07 週 セキュリティニュースメモ"
emoji: "🎋"
type: "tech"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。早いのはGitHubです
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威

* 2023/10 のJAXA不正アクセス、起点は、VPN
    * https://www.security-next.com/159383
    * https://www.jaxa.jp/press/2024/07/20240705-2_j.html

# 脆弱性
* CVE-2024-34750 Apache Tomcat DoSの脆弱性
    * https://jvn.jp/vu/JVNVU90387090/index.html
    * https://www.security-next.com/159421
* CVE-2024-36991 Splunk パスとラバーサルの脆弱性
    * https://nvd.nist.gov/vuln/detail/CVE-2024-36991
    * https://github.com/bigb0x/CVE-2024-36991
* CVE-2024-39202 D-Link Router RCE PoCあり
    * https://gist.github.com/Swind1er/40c33f1b1549028677cb4e2e5ef69109
* CVE-2024-6387 regreSSHion, 複数のCisco製品で修正
    * https://securityonline.info/cisco-confirms-critical-openssh-regresshion-cve-2024-6387-flaw-in-multiple-products/
    * https://www.security-next.com/159425
* CVE-2024-39349 Synology Camera 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-39349-cvss-9-8-critical-vulnerability-in-synology-surveillance-cameras/

# その他
* Google ダークウェブレポート を無料開放
    * https://forest.watch.impress.co.jp/docs/news/1606361.html
* AppleStoreからいくつかのロシアのVPNアプリが削除される
    * https://www.bleepingcomputer.com/news/technology/russia-forces-apple-to-remove-dozens-of-vpn-apps-from-app-store/
    * https://thehackernews.com/2024/07/apple-removes-vpn-apps-from-russian-app.html
* Windows11 Notepad.exeにスペルチェックとオートコレクトが、すべてのユーザに実装
    * https://www.bleepingcomputer.com/news/microsoft/notepad-finally-gets-spellcheck-autocorrect-for-all-windows-11-users/
    * https://www.theregister.com/2024/07/08/it_only_took_41_years/
* Windows11 22H2 EOLが今年の10月
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-11-22h2-reaches-end-of-service-in-october/
