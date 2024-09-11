---
title: "2024/09/08 週 セキュリティニュースメモ"
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

# 脆弱性

* CVE-2024-24759 AI等で利用されているMindsDB、SSRFの脆弱性
    * https://securityonline.info/mindsdb-fixes-critical-cve-2024-24759-dns-rebinding-attack-bypasses-security-protections/
* CVE-2024-37288 and CVE-2024-37285 Kibana 任意のコード実行
    * https://securityonline.info/critical-kibana-flaws-cve-2024-37288-cve-2024-37285-expose-systems-to-arbitrary-code-execution/
    * https://rocket-boys.co.jp/8076/
* CVE-2024-26230 Windows 4月に修正された権限昇格の脆弱性のPoC公開
    * https://securityonline.info/poc-exploit-releases-for-windows-elevation-of-privilege-vulnerability-cve-2024-26230/
* CVE-2024-29847 Ivanti EPM 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/ivanti-fixes-maximum-severity-rce-bug-in-endpoint-management-software/
    * https://securityonline.info/ivanti-issues-patch-for-critical-vulnerabilities-in-endpoint-manager-including-cve-2024-29847-cvss-10-0/
* CVE-2024-41869 CVE-2024-45112 Adobe Acrobat Reader 他 任意のコード実行の脆弱性
    * https://helpx.adobe.com/security/products/acrobat/apsb24-70.html
    * https://www.securityweek.com/adobe-patches-critical-code-execution-flaws-in-multiple-products/
* CVE-2024-7889 and CVE-2024-7890 Citrix Workspace app for Windows 権限昇格の脆弱性
    * https://support.citrix.com/s/article/CTX691485-citrix-workspace-app-for-windows-security-bulletin-cve20247889-and-cve20247890?language=en_US
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Sep
        * https://krebsonsecurity.com/2024/09/bug-left-some-windows-pcs-dangerously-unpatched/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-windows-server-performance-issues-from-august-updates/
        * https://www.securityweek.com/microsoft-says-windows-update-zero-day-being-exploited-to-undo-security-fixes/
        * https://www.bleepingcomputer.com/news/microsoft/windows-10-kb5043064-update-released-with-6-fixes-security-updates/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-september-2024-patch-tuesday-fixes-4-zero-days-79-flaws/
* KEV
    * CVE-2016-3714 ImageMagick Improper Input Validation Vulnerability
    * CVE-2017-1000253 Linux Kernel PIE Stack Buffer Corruption Vulnerability
    * CVE-2024-40766 SonicWall SonicOS Improper Access Control Vulnerability
        * https://jp.inoreader.com/article/3a9c6e745fcd536b-akira-ransomware-exploits-sonicwall-sslvpn-flaw-cve-2024-40766
        * https://www.darkreading.com/ics-ot-security/akira-ransomware-actors-exploit-sonicwall-bug-for-rce
        * https://www.security-next.com/161650
        * https://www.bleepingcomputer.com/news/security/critical-sonicwall-sslvpn-bug-exploited-in-ransomware-attacks/
    * CVE-2024-38226 Microsoft Publisher Security Feature Bypass Vulnerability
    * CVE-2024-43491 Microsoft Windows Update Remote Code Execution Vulnerability
    * CVE-2024-38014 Microsoft Windows Installer Privilege Escalation Vulnerability
    * CVE-2024-38217 Microsoft Windows Mark of the Web (MOTW) Security Feature Bypass Vulnerability
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-windows-smart-app-control-zero-day-exploited-since-2018/

# その他

* NGINX GitHubへ移行
    * https://forest.watch.impress.co.jp/docs/news/1622344.html
    * https://securityonline.info/nginx-open-source-makes-the-jump-to-github-boosting-collaboration-and-community-engagement/
* カスペルスキー、米国事業縮小に関連して、移行先UltraAVを案内
    * https://www.securityweek.com/one-million-us-kaspersky-customers-transferred-to-pangos-ultraav/
* Windows 22H2 を23H2 に強制アップグレードすることを発表。10/8を予定
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-start-force-upgrading-windows-22h2-systems-next-month/
