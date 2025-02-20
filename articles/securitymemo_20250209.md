---
title: "2025/02/09 週 セキュリティニュースメモ"
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

* CVE-2025-24200 iOSデバイス USB制限モードへの脆弱性。extremely sophisticated
    * https://www.bleepingcomputer.com/news/apple/apple-fixes-zero-day-exploited-in-extremely-sophisticated-attacks/
    * https://securityonline.info/apple-issues-emergency-updates-to-patch-actively-exploited-zero-day-vulnerability-cve-2025-24200/
    * https://thehackernews.com/2025/02/apple-patches-actively-exploited-ios.html
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/apple-emergency-ios-18-3-1-extremely-sophisticated-attack-update-now
* CVE-2025-23369 GitHub Enterprise SAML Bypass
    * https://securityonline.info/github-enterprise-saml-bypass-flaw-cve-2025-23369-exposed-technical-analysis-and-exploit-poc/
* CVE-2024-47908 Ivanti CSA 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-47908-cvss-9-1-critical-ivanti-csa-flaw-enables-attackers-to-run-arbitrary-code/
* CVE-2025-22467 Ivanti Connect Secure 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2025-22467-cvss-9-9-ivanti-connect-secure-vulnerability-allows-remote-code-execution/
* CVE-2024-54531 macOS 昨年12月に修正されたKASLR Bypassの脆弱性、PoCリリース
    * https://securityonline.info/macos-security-breach-cve-2024-54531-poc-published-attackers-can-bypass-kaslr/
* CVE-2025-0108 Paloalto PAN-OS 未認証のアクセスの脆弱性
    * https://securityonline.info/cve-2025-0108-cve-2025-0110-palo-alto-networks-fixes-high-severity-pan-os-vulnerabilities/
    * https://www.bleepingcomputer.com/news/security/hackers-exploit-authentication-bypass-in-palo-alto-networks-pan-os/
    * PoCリリース
        * https://securityonline.info/palo-alto-firewall-flaw-cve-2025-0108-active-exploits-in-the-wild-poc-released/
    * https://www.theregister.com/2025/02/19/palo_alto_firewall_attack/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-Feb
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-february-2025-patch-tuesday-fixes-4-zero-days-55-flaws/
        * https://www.securityweek.com/microsoft-patches-wormable-windows-flaw-and-file-deleting-zero-day/

## KEV
* CVE-2024-40891 Zyxel DSL CPE OS Command Injection Vulnerability
* CVE-2024-40890 Zyxel DSL CPE OS Command Injection Vulnerability
* CVE-2025-21418 Microsoft Windows Ancillary Function Driver for WinSock Heap-Based Buffer Overflow Vulnerability
* CVE-2025-21391 Microsoft Windows Storage Link Following Vulnerability
* CVE-2024-57727 SimpleHelp Path Traversal Vulnerability

# その他
* Google Youtube Userのメールアドレスが漏れる不具合を修正
    * https://www.bleepingcomputer.com/news/security/google-fixes-flaw-that-could-unmask-youtube-users-email-addresses/
