---
title: "2025/01/05 週 セキュリティニュースメモ"
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

* NessusAgent ダウン。プラグイン更新により
    * https://www.bleepingcomputer.com/news/security/bad-tenable-plugin-updates-take-down-nessus-agents-worldwide/
* CASIO 昨年10月のランサムウェア被害、約8,500人の顧客情報流出を認める
    * https://www.bleepingcomputer.com/news/security/casio-says-data-of-8-500-people-exposed-in-october-ransomware-attack/
    * https://news.google.com/rss/articles/CBMiXkFVX3lxTE9kT2RKME1iZWpObjhzWk1KZXVndmtZRmF1UlRhVnlMRUtMREdQSjVrM2ZyQmIwVHozdWxaWUhFbkdhcHROVGVJd3V0dExoX1VfUzN6QmFScUdGcFFBZFE?oc=5&hl=en-US&gl=US&ceid=US:en
    * https://www.itmedia.co.jp/news/articles/2501/07/news179.html
    * https://www.securityweek.com/thousands-impacted-by-casio-data-breach/
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/casios-october-ransomware-attack-leads-to-personal-data-leak
* りそな銀行 再び、繋がりづらい状態
    * https://news.goo.ne.jp/picture/business/tbs-1654021.html
    * https://www.nnn.co.jp/articles/-/452712
* Proton Mail世界的にサービス障害
    * https://www.bleepingcomputer.com/news/technology/proton-mail-still-down-as-proton-recovers-from-worldwide-outage/
* 三菱UFJでシステム障害、他行ATMで出金できず　「サイバー攻撃ではない」
    * https://www.sankei.com/article/20250109-4YWVMVJWTJOP3L5WDICDLSVXRU/
    * https://www.fnn.jp/articles/-/812255



# 攻撃、脅威



# 脆弱性

* CVE-2024-51741 and CVE-2024-46981 Redis DoSの脆弱性
    * https://securityonline.info/cve-2024-51741-and-cve-2024-46981-redis-flaws-expose-millions-to-dos-and-rce-risks/
* CVE-2024-43096 Android RCEの脆弱性
    * https://securityonline.info/cve-2024-43096-and-more-critical-rce-flaws-patched-in-android-security-update/
* CVE-2024-43452 昨年11月に修正されたWindows権限昇格の脆弱性 PoCリリース
    * https://securityonline.info/cve-2024-43452-poc-exploit-released-for-windows-elevation-of-privilege-bug/#google_vignette
* CVE-2024-53704 SonicWALL SSLVPNやSSH管理に関して認証bypassの脆弱性
    * https://www.bleepingcomputer.com/news/security/sonicwall-urges-admins-to-patch-exploitable-sslvpn-bug-immediately/
* CVE-2024-52316 Apache Tomcatの認証bypassの脆弱性、DELLのOpenManagerへも影響あり
    * https://securityonline.info/authentication-bypass-vulnerability-found-in-dell-openmanage-server-administrator/
* 「Node.js」のEOL版に重大な脆弱性。CVE再番予定
    * https://www.security-next.com/165966
    * https://nodejs.org/en/blog/vulnerability/upcoming-cve-for-eol-versions

## KEV
* CVE-2024-41713 Mitel MiCollab Path Traversal Vulnerability
* CVE-2024-55550 Mitel MiCollab Path Traversal Vulnerability
* CVE-2020-2883 Oracle WebLogic Server Unspecified Vulnerability
* CVE-2025-0282 Ivanti Connect Secure Vulnerability
    * https://www.bleepingcomputer.com/news/security/ivanti-warns-of-new-connect-secure-flaw-used-in-zero-day-attacks/
    * https://www.security-next.com/165969
    * https://www.bleepingcomputer.com/news/security/google-chinese-hackers-likely-behind-ivanti-vpn-zero-day-attacks/

# その他

* インド、WARPを含むVPNソフトウェア、アプリストアから削除(撤退)。インド政府のログ保管要件に合わず
    * https://securityonline.info/indias-vpn-crackdown-popular-apps-vanish-from-app-stores/
