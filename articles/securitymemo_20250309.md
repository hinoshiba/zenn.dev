---
title: "2025/03/09 週 セキュリティニュースメモ"
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

# 攻撃、脅威

# 脆弱性

* CVE-2025-27607 python-json-logger 任意のコード実行の可能性
    * https://securityonline.info/popular-python-logging-library-vulnerable-to-remote-code-execution-cve-2025-27607/
* CVE-2024-50394 QNAP helpdesk app 遠隔からのアクセスの脆弱性
    * https://securityonline.info/cve-2024-50394-qnap-helpdesk-vulnerability-could-allow-remote-system-compromise/#google_vignette
* CVE-2025-0337 ServiceNOW 未認証のアクセス
    * https://securityonline.info/servicenow-addresses-authorization-bypass-vulnerability-in-now-platform-cve-2025-0337/
* CVE-2025-1316 Edimax IC-7100 IP 任意のコード実行の脆弱性。CIA警告
    * https://securityonline.info/cisa-warns-of-critical-edimax-ip-camera-flaw-cve-2025-1316-with-public-exploits-and-no-vendor-fix/
    * https://www.securityweek.com/edimax-says-no-patches-coming-for-zero-day-exploited-by-botnets/
* CVE-2025-20206: Cisco Secure Client 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2025-20206-cisco-secure-client-flaw-allows-code-execution-with-system-privileges/
* CVE-2025-27624 Jenkins CSRF
    * https://securityonline.info/csrf-and-open-redirect-jenkins-patches-major-vulnerabilities/
* CVE-2025-0912 GiveWP 任意のコード実行
    * https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/give/givewp-donation-plugin-and-fundraising-platform-3194-unauthenticated-php-object-injection
* CVE-2024-56337 Apache Tomcat レースコンディションによりファイルをJSPとして利用される可能性
    * https://www.security-next.com/168002
* CVE-2025-24813 Apache Tomcat 任意のコード実行の可能性。PoCリリース
    * https://securityonline.info/cve-2025-24813-flaw-in-apache-tomcat-exposes-servers-to-rce-data-leaks-update-immediately/
    * https://securityonline.info/tomcat-flaw-cve-2025-24813-exploited-in-the-wild-poc-released/#google_vignette
    * https://github.com/iSee857/CVE-2025-24813-PoC
    * https://www.darkreading.com/vulnerabilities-threats/apache-tomcat-rce-vulnerability-exploit
    * https://www.securityweek.com/exploit-code-for-apache-tomcat-rce-vulnerability-published-on-chinese-forum/
    * https://thehackernews.com/2025/03/apache-tomcat-vulnerability-comes-under.html
    * https://www.bleepingcomputer.com/news/security/critical-rce-flaw-in-apache-tomcat-actively-exploited-in-attacks/
* CVE-2025-24201 Apple device Webkitの脆弱性
    * https://www.darkreading.com/mobile-security/apple-drops-another-webkit-zero-day-bug
    * https://thehackernews.com/2025/03/apple-releases-patch-for-webkit-zero.html
    * https://securityonline.info/cve-2025-24201-apple-issues-emergency-patches-for-actively-exploited-zero-day-vulnerability/
    * https://www.bleepingcomputer.com/news/apple/apple-fixes-webkit-zero-day-exploited-in-extremely-sophisticated-attacks/
* CVE-2025-27440 Zoom 権限昇格の脆弱性
    * https://www.securityweek.com/zoom-patches-4-high-severity-vulnerabilities/
    * https://securityonline.info/zoom-addresses-multi-high-severity-vulnerabilities-in-workplace-apps-and-sdks/
* CVE-2023-40723 ForiSIEM 遠隔からのDB情報読み取りの可能性
    * https://www.securityweek.com/fortinet-patches-18-vulnerabilities/
* CVE-2025-26865 Apache OfBiz RCE
    * https://securityonline.info/cve-2025-26865-apache-ofbiz-vulnerability-could-lead-to-remote-code-execution/
* CVE-2025-21590 Juniper Junos RCE
    * https://www.bleepingcomputer.com/news/security/juniper-patches-bug-that-let-chinese-cyberspies-backdoor-routers-since-mid-2024/
    * https://securityonline.info/juniper-issues-urgent-fix-for-actively-exploited-junos-os-flaw-cve-2025-21590/
* CVE-2025-25291 and CVE-2025-25292 RubySAML Bypassの脆弱性。GitLabやGitHubにも影響あり
    * https://www.bleepingcomputer.com/news/security/gitlab-patches-critical-authentication-bypass-vulnerabilities/
    * https://thehackernews.com/2025/03/github-uncovers-new-ruby-saml.html
    * https://securityonline.info/gitlab-urgently-patches-critical-authentication-bypass-flaws-cve-2025-25291-cve-2025-25292/
* CVE-2025-20138 Cisco IOS XR
    * https://securityonline.info/cisco-issues-high-severity-security-alert-for-ios-xr-software-cve-2025-20138/
* CVE-2025-27017 Apache NiFi 未認証のDBアクセス
    * https://securityonline.info/cve-2025-27017-apache-nifi-vulnerability-exposes-mongodb-credentials/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-Mar
        * https://securityboulevard.com/2025/03/microsofts-march-2025-patch-tuesday-addresses-56-cves-cve-2025-26633-cve-2025-24983-cve-2025-24993/
        * https://securityonline.info/microsoft-patch-tuesday-march-2025-addresses-67-vulnerabilities-including-seven-zero-day-flaws/

## KEV
* CVE-2025-25181 Advantive VeraCore SQL Injection Vulnerability
* CVE-2024-57968 Advantive VeraCore Unrestricted File Upload Vulnerability
* CVE-2024-13159 Ivanti Endpoint Manager (EPM) Absolute Path Traversal Vulnerability
* CVE-2024-13160 Ivanti Endpoint Manager (EPM) Absolute Path Traversal Vulnerability
* CVE-2024-13161 Ivanti Endpoint Manager (EPM) Absolute Path Traversal Vulnerability
* CVE-2025-24201 Apple Multiple Products WebKit Out-of-Bounds Write Vulnerability
* CVE-2025-21590 Juniper Junos OS Improper Isolation or Compartmentalization Vulnerability

# その他

* MicrosoftがリモートデスクトップアプリをWindowsAppに切り替えていく
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-replacing-remote-desktop-app-with-windows-app-in-may/
* GCC 15のリリース間近
    * https://www.theregister.com/2025/03/13/gcc_15_is_close/
