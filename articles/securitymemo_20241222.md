---
title: "2024/12/22 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

* アメリカン航空が米国で全便運航停止、約1時間後に解除　技術障害
    * https://jp.reuters.com/markets/japan/funds/TCPP4O2A3NKV3KT7G6OWORSHBQ-2024-12-24/
* ＤＭＭビットコインの不正流出、北朝鮮系グループが関与＝警察庁
    * https://jp.reuters.com/markets/japan/funds/VB4JLA2RHZKRJGOCRGAE6P6OAU-2024-12-23/

# 攻撃、脅威

* JAL システム障害
    * https://databreaches.net/2024/12/26/japan-airlines-recovers-from-cyberattack-confirms-no-customer-data-leaks/
    * https://www.securityweek.com/japan-airlines-was-hit-by-a-cyberattack-delaying-flights-during-the-year-end-holiday-season/
    * https://news.mynavi.jp/techplus/article/20241227-3095482/
    * https://www3.nhk.or.jp/lnews/oita/20241226/5070020300.html

# 脆弱性

* CVE-2024-3393 PaloAlto 未認証のDoSの脆弱性。DNSセキュリティ機能に起因
    * https://www.bleepingcomputer.com/news/security/hackers-exploit-dos-flaw-to-disable-palo-alto-networks-firewalls/
    * https://security.paloaltonetworks.com/CVE-2024-3393
    * https://thehackernews.com/2024/12/palo-alto-releases-patch-for-pan-os-dos.html
    * https://securityonline.info/cve-2024-3393-pan-os-vulnerability-now-exploited-in-the-wild/
* CVE-2024-52046 Apache MINA RCE
    * https://thehackernews.com/2024/12/apache-mina-cve-2024-52046-cvss-100.html
    * https://securityonline.info/cve-2024-52046-cvss-10-critical-apache-mina-flaw-could-allow-remote-code-execution/
* CVE-2024-40896 libxml2 XXE
    * https://securityonline.info/cve-2024-40896-cvss-9-1-critical-xxe-vulnerability-discovered-in-libxml2/
    * https://www.security-next.com/165738
* CVE-2024-45387 Apache Traffic Control SQLi
    * https://thehackernews.com/2024/12/critical-sql-injection-vulnerability-in.html
    * https://www.security-next.com/165656
* CVE-2024-30085 6月に修正されたWindows権限昇格の意是弱生、PoCリリース
    * https://securityonline.info/poc-exploit-released-for-cve-2024-30085-windows-elevation-of-privilege-vulnerability/
* CVE-2024-53961 Adobe ColdFusion 緊急度の高い脆弱性。PoC及びセキュリティパッチをリリース
    * https://www.bleepingcomputer.com/news/security/adobe-warns-of-critical-coldfusion-bug-with-poc-exploit-code/
* CVE-2024-56046 WordPress WPLMSテーマ、RCEの脆弱性
    * https://www.bleepingcomputer.com/news/security/premium-wplms-wordpress-plugins-address-seven-critical-flaws/

# その他

* Cloudflare WARP のVPNプロトコルにMASQUEを追加。DEXも一般リリース
    * https://blog.cloudflare.com/masque-now-powers-1-1-1-1-and-warp-apps-dex-available-with-remote-captures/
* ASUSのクリスマスキャンペーンに避難
    * https://news.mynavi.jp/techplus/article/20241225-3093971/
    * https://www.windowslatest.com/2024/12/22/asus-bombards-windows-11-with-christmas-exe-malware-like-christmas-wreath-banner/
