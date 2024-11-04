---
title: "2024/10/27 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
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
* デルタ航空、Crowdstrikeに対して $500Milion の起訴
    * https://www.darkreading.com/cyberattacks-data-breaches/delta-launches-500m-lawsuit-crowdstrike

# 攻撃、脅威
* 「出前館」が3日間にわたりサービス停止 - マルウェア感染で
    https://www.security-next.com/163603
* シャープ公式オンラインストア｢COCORO STORE｣・食材宅配サービス｢ヘルシオデリ｣における不正アクセスによる個人情報流出に関するお詫びと調査結果のお知らせ
    * https://corporate.jp.sharp/info/notices/241030-a.html


# 脆弱性

* CVE-2024-9488 WordPress Plugin wpDiscuz 認証bypassの脆弱性
    * https://securityonline.info/cve-2024-9488-cvss-9-8-authentication-bypass-flaw-in-wpdiscuz-plugin-over-80000-sites-at-risk/
* Windowsのダウングレード攻撃、修正済みのWindowsで実証
    * https://thehackernews.com/2024/10/researchers-uncover-os-downgrade.html
    * https://news.mynavi.jp/techplus/article/20241028-3053962/
    * https://innovatopia.jp/cyber-security/cyber-security-news/44153/
* CVE-2024-50387 QNAP NAS root権限を取得できる脆弱性
    * https://www.bleepingcomputer.com/news/security/qnap-patches-second-zero-day-exploited-at-pwn2own-to-get-root/
    * https://securityonline.info/cve-2024-50387-critical-qnap-flaw-exploited-in-hacking-contest-patch-now/
    * https://securityonline.info/qnap-patches-critical-zero-day-exploited-at-pwn2own-ireland-2024-cve-2024-50388/
    * https://www.bleepingcomputer.com/news/security/qnap-fixes-nas-backup-software-zero-day-exploited-at-pwn2own/
    * https://www.security-next.com/163670
* CVE-2024-45802 Squid Edge Side Includes (ESI)機能が有効な場合、DoSの脆弱性の影響
    * https://securityonline.info/denial-of-service-vulnerability-found-in-squid-proxy-server-cve-2024-45802/
* CVE-2024-45656 IBM Power Systems server 任意のアクセスが可能となる脆弱性
    * https://securityonline.info/cve-2024-45656-a-9-8-severity-threat-to-ibm-power-systems-security/
* Windowsのテーマに関する脆弱性で、NTML情報を盗めるもの。非公式パッチが配布されている
    * https://www.bleepingcomputer.com/news/security/new-windows-themes-zero-day-gets-free-unofficial-patches/
    * https://www.theregister.com/2024/10/30/zeroday_windows_themes/
* CVE-2024-38821 Spring WebFlux 認証bypassの脆弱性
    * https://securityonline.info/cve-2024-38821-cvss-9-1-allows-authorization-bypass-in-webflux-applications/
    * https://securityonline.info/poc-exploit-releases-for-spring-webflux-authorization-bypass-cve-2024-38821/
* CVE-2024-50550 WordPress Plugin LiteSpeedCache 未認証の管理者アクセスの脆弱性
    * https://www.bleepingcomputer.com/news/security/litespeed-cache-wordpress-plugin-bug-lets-hackers-get-admin-access/
    * https://thehackernews.com/2024/10/litespeed-cache-plugin-vulnerability.html
* CVE-2024-10392 WordPress Plugin AI Power 任意のコード実行の脆弱性
    * https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/gpt3-ai-content-generator/ai-power-complete-ai-pack-1889-unauthenticated-arbitrary-file-upload
    https://securityonline.info/cve-2024-10392-cvss-9-8-popular-wordpress-ai-plugin-exposed-to-critical-security-risk/
* CVE-2024-10443 Synology NAS 任意のコード実行の脆弱性。PoCなし
    * https://x.com/thezdi/status/1849068671177531664
    * https://www.bleepingcomputer.com/news/security/synology-fixed-two-critical-zero-days-exploited-at-pwn2own-within-days/
* CVE-2024-10487 GoogleChrome領域外書き込みの脆弱性
    * https://www.bitdefender.com/en-gb/blog/hotforsecurity/patch-browser-google-updates-chrome-critical-bug-fixes/
* CVE-2024-9632 X.Org Server RCEやDoSの脆弱性
    * https://securityonline.info/cve-2024-9632-18-year-old-bug-in-x-org-server-leaves-systems-vulnerable-to-attack/

# その他

* Exchange Online向けの受信SMTP DANEおよびDNSSECの一般提供開始
    * https://techcommunity.microsoft.com/t5/exchange-team-blog/announcing-general-availability-of-inbound-smtp-dane-with-dnssec/ba-p/4281292
    * https://securityonline.info/microsoft-boosts-email-security-with-general-availability-of-inbound-smtp-dane-with-dnssec/
* Windows 10ユーザは、$30を支払うことで来年も Extended Security Updatesを受けられ、Windows11へのアップグレードを遅延させることができる
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-wants-30-if-you-want-to-delay-windows-11-switch/
* Windows11 タスクマネージャで誤ったプロセスIDが表示される不具合。10月のプレビューアップデート以降。
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-task-manager-bug-shows-wrong-number-of-running-processes/
