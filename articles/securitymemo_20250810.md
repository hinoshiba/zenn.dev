---
title: "2025/08/10 週 セキュリティニュースメモ"
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

* 駿河屋 第三者不正アクセスによる個人情報漏えいとクレジットカード決済停止に関するお詫びとお知らせ / ECサイト改ざんによるクレジットカード情報窃取の可能性
    * https://www.suruga-ya.jp/feature/osirase/2025_08_08.html
    * https://news.yahoo.co.jp/articles/2848fad0c527f4fe26988382f7a2e6ce389fe754

# 攻撃、脅威

* ひらがなの「ん」を用いたpunicodeのフィッシングメール
    * https://www.bleepingcomputer.com/news/security/bookingcom-phishing-campaign-uses-sneaky-character-to-trick-you/

# 脆弱性

* CVE-2025-8088 WinRAR Zero-Day
    * https://dailydarkweb.net/winrar-zero-day-vulnerability-allegedly-exploited-by-russian-hackers-to-target-governments/
    * https://www.securityweek.com/russian-hackers-exploited-winrar-zero-day-in-attacks-on-europe-canada/
    * https://thehackernews.com/2025/08/winrar-zero-day-under-active.html
    * https://securityonline.info/winrar-update-zero-day-path-traversal-flaw-cve-2025-8088-actively-exploited-to-deliver-malware/
    * https://codebook.machinarecord.com/threatreport/silobreaker-cyber-alert/40252/
* CVE-2025-38236 Linux 権限昇格の脆弱性
    * https://securityonline.info/linux-kernel-flaw-privilege-escalation-risk-poc-code-available/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-aug
        * https://krebsonsecurity.com/2025/08/microsoft-patch-tuesday-august-2025-edition/
* CVE-2025-25256 FortiSIEM 未認証のコード実行
    * https://www.bleepingcomputer.com/news/security/fortinet-warns-of-fortisiem-pre-auth-rce-flaw-with-exploit-in-the-wild/
    * https://thehackernews.com/2025/08/fortinet-warns-about-fortisiem.html
    * https://securityonline.info/fortisiem-cve-2025-25256-cvss-9-8-remote-unauthenticated-command-injection-with-exploit-in-the-wild/
* CVE-2025-7734 GitLab BobViewer上でのXSSの脆弱性
    * https://securityonline.info/gitlab-patches-high-severity-flaws-update-now-to-prevent-xss-and-account-takeover/
* CVE-2025-49457 Zoom Windows 権限昇格の脆弱性
    * https://securityonline.info/zoom-patches-critical-flaw-cve-2025-49457-windows-users-face-privilege-escalation-risk/

## KEV
* CVE-2013-3893 Microsoft Internet Explorer Resource Management Errors Vulnerability
* CVE-2007-0671 Microsoft Office Excel Remote Code Execution Vulnerability
* CVE-2025-8088 RARLAB WinRAR Path Traversal Vulnerability

# その他

* Windows 365 Reserve Public Preview
    * https://techcommunity.microsoft.com/blog/windows-itpro-blog/enhancing-business-continuity-windows-365-reserve-is-now-in-limited-public-previ/4441669
* IPA スペシャリスト区分試験をCBTへ移行予定2026年度から。
    * https://www.ipa.go.jp/shiken/2026/ap_koudo_sc-cbt.html
