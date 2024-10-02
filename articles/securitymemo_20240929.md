---
title: "2024/09/29 週 セキュリティニュースメモ"
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

# 攻撃、脅威

* シンガポールヤマト運輸に不正アクセス、他のヤマトグループへの影響は確認されず
    * https://scan.netsecurity.ne.jp/article/2024/09/25/51656.html
* T-Mobile FCCへ民事罰金$15.75 million
    * https://www.theregister.com/2024/09/30/tmobile_data_breaches_settlement/
    * https://www.bleepingcomputer.com/news/security/t-mobile-pays-315-million-fcc-settlement-over-4-data-breaches/
    * https://www.securityweek.com/t-mobile-to-pay-millions-to-settle-with-fcc-over-data-breaches/

# 脆弱性
* CVE-2024-8926 PHP Parameter Injection の脆弱性
    * https://securityonline.info/multiple-vulnerabilities-discovered-in-php-prompting-urgent-security-updates/
* CVE-2024-8353 WordPress Plugin GiveWP PHP Object Injection
    * https://securityonline.info/cve-2024-8353-critical-givewp-flaw-100k-wordpress-sites-at-risk/  
    * https://www.security-next.com/162401
* CVE-2024-45489 Arch ブラウザ。任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/arc-browser-launches-bug-bounty-program-after-fixing-rce-bug/
* CVE-2024-45519 Zimbra 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/critical-zimbra-rce-flaw-exploited-to-backdoor-servers-using-emails/


## KEV
* CVE-2024-29824 Ivanti Endpoint Manager (EPM) SQL Injection Vulnerability
* CVE-2023-25280 D-Link DIR-820 Router OS Command Injection Vulnerability
* CVE-2020-15415 DrayTek Multiple Vigor Routers OS Command Injection Vulnerability
* CVE-2021-4043 Motion Spell GPAC Null Pointer Dereference Vulnerability
* CVE-2019-0344 SAP Commerce Cloud Deserialization of Untrusted Data Vulnerability

# その他

* MicrosoftDefender 安全でないWifi接続時に警告をだしDefenderVPNへの接続を促す機能を追加 
    * https://www.bleepingcomputer.com/news/security/microsoft-defender-now-automatically-detects-unsecure-wi-fi-networks/
* ブラジル X再開前に罰金
    * https://jp.reuters.com/economy/industry/QU4MYMV3RRPFRJHAI6BBERHDNM-2024-09-30/ 
* Verizon ダウン。iPhoneは、SOSモードになり続ける
    * https://www.bleepingcomputer.com/news/technology/iphones-android-devices-stuck-in-sos-mode-after-verizon-outage/    
* 400近いエプソン製プリンタやスキャナに脆弱性 - 管理者パスワードの設定を
    * https://www.security-next.com/162404
* Pマークのオンライン申請を受付開始 - JIPDEC
    * https://www.security-next.com/162468
* iOS 18に関するセキュリティtpis
    * https://scotthelme.co.uk/ios-18-quick-tips-security-edition/
* 9月上旬の大規模DDoSに関するレポート @Cloudflare
    * https://blog.cloudflare.com/how-cloudflare-auto-mitigated-world-record-3-8-tbps-ddos-attack/
* Microsoft Office 2024 リリース
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-office-2024-now-available-for-windows-and-macos-no-subscription-required/
