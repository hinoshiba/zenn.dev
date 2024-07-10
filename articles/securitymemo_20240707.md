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
* CVE-2024-5441 WordPress Plugin Modern Events Calendar RCE
    * https://www.bleepingcomputer.com/news/security/hackers-target-wordpress-calendar-plugin-used-by-150-000-sites/
* CVE-2024-3596 RADIUS プロトコル MitMの可能性
    * https://www.cvedetails.com/cve/CVE-2024-3596/?q=CVE-2024-3596
    * https://kb.cert.org/vuls/id/456537
* CVE-2024-6409 OpenSSH RCEの脆弱性
    * https://securityonline.info/cve-2024-6409-new-remote-code-execution-vulnerability-in-openssh/
    * https://www.security-next.com/159488
* CVE-2024-22274 vCentor リモートから乗っ取られる可能性
    * https://securityonline.info/vmware-vcenter-server-rce-cve-2024-22274-poc-exposes-systems-to-remote-takeover/
* CVE-2024-5491 CVE-2024-5492 NetScaler ADC and NetScaler Gateway Security Bulletin 未認証のユーザが他ユーザを誘導する可能性やDoS
    * https://support.citrix.com/article/CTX677944/netscaler-adc-and-netscaler-gateway-security-bulletin-for-cve20245491-and-cve20245492%20%20
* CVE-2024-34123 Adobe Premiere Pro  信頼できないPATH探索の脆弱性
    * https://helpx.adobe.com/security/products/premiere_pro/apsb24-46.html
    * https://www.securityweek.com/adobe-issues-critical-patches-for-multiple-products-warns-of-code-execution-risks/
* WindowsUpdate
    * info
        * https://www.securityweek.com/microsoft-warns-of-windows-hyper-v-zero-day-being-exploited/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-july-2024-patch-tuesday-fixes-142-flaws-4-zero-days/
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Jul
        * https://msrc.microsoft.com/update-guide/vulnerability
    * publicly disclosed / exploited
        * CVE-2024-37985 Arm: CVE-2024-37985 Systematic Identification and Characterization of Proprietary Prefetchers
        * CVE-2024-35264 .NET and Visual Studio Remote Code Execution Vulnerability
        * CVE-2023-38545 Hackerone: CVE-2023-38545 SOCKS5 heap buffer overflow
        * CVE-2023-24932 Secure Boot Security Feature Bypass Vulnerability
        * CVE-2024-38112 Windows MSHTML Platform Spoofing Vulnerability
        * CVE-2024-38080 Windows Hyper-V Elevation of Privilege Vulnerability
    * CVSS 9.x
        * CVE-2024-38074 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38076 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38077 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38089 Microsoft Defender for IoT Elevation of Privilege Vulnerability
* KEV
    * CVE-2024-23692 Rejetto HTTP File Server Improper Neutralization of Special Elements Used in a Template Engine Vulnerability
    * CVE-2024-38080 Microsoft Windows Hyper-V Privilege Escalation Vulnerability
    * CVE-2024-38112 Microsoft Windows MSHTML Platform Spoofing Vulnerability

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
