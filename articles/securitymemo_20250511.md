---
title: "2025/05/11 週 セキュリティニュースメモ"
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

* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-mar
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-may-2025-patch-tuesday-fixes-5-exploited-zero-days-72-flaws/
        * https://securityonline.info/microsoft-may-2025-patch-tuesday-fixes-83-vulnerabilities-including-5-exploited-in-the-wild/
    * CVE-2025-30397 Scripting Engine Memory Corruption Vulnerability
        * https://www.darkreading.com/vulnerabilities-threats/windows-zero-day-bug-exploited-browser-rce
* CVE-2025-31324 SAP 未認証のファイルアップロード
    * https://www.bleepingcomputer.com/news/security/sap-patches-second-zero-day-flaw-exploited-in-recent-attacks/
* CVE-2025-4427 Ivanti コード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/ivanti-fixes-epmm-zero-days-chained-in-code-execution-attacks/

* CVE-2024-45332 Intel CPU 特権メモリ領域から機密データの漏洩の可能性
    * https://www.bleepingcomputer.com/news/security/new-intel-cpu-flaws-leak-sensitive-data-from-privileged-memory/
* CVE-2025-31258 macOS RemoteViewSerivceを利用してSandboxEscapeの脆弱性
    * https://securityonline.info/poc-released-cve-2025-31258-sandbox-escape-in-macos-via-remoteviewservices/
    * https://www.microsoft.com/en-us/security/blog/2025/05/01/analyzing-cve-2025-31191-a-macos-security-scoped-bookmarks-based-sandbox-escape/
* CVE-2025-46802 GNU Screen TTY ハイジャック
    * https://securityonline.info/multiple-cves-in-gnu-screen-local-root-exploit-and-tty-hijacking-discovered/
* CVE-2025-31644 BIG-IP アプリケーションモード経由により管理者権限の奪取の可能性
    * https://securityonline.info/poc-released-cve-2025-31644-exploit-grants-root-access-on-f5-big-ip-via-appliance-mode-command-injection/
* CVE-2025-3462 ASUS DriverHub 悪意のあるコマンド実行の可能性
    * https://www.bleepingcomputer.com/news/security/asus-driverhub-flaw-let-malicious-sites-run-commands-with-admin-rights/
    * https://thehackernews.com/2025/05/asus-patches-driverhub-rce-flaws.html
    * https://securityonline.info/critical-security-flaws-found-in-asus-driverhub-update-immediately/
* CVE-2025-4641 Selemium XXE の脆弱性
    * https://securityonline.info/popular-selenium-library-webdrivermanager-hit-by-critical-xxe-bug-cve-2025-4641-cvss-9-3/
* CVE-2025-32002 IO-DATA NAS RCEの脆弱性
    * https://securityonline.info/critical-nas-risk-i-o-data-flaw-with-9-8-cvss-allows-remote-command-execution/
* BitLockerの暗号化をbypassする手法に関するレポート
    * https://securityonline.info/bitlocker-encryption-bypassed-in-minutes-via-bitpixie-cve-2023-21563-poc-reveals-high-risk-attack-path/
    * https://blog.compass-security.com/2025/05/bypassing-bitlocker-encryption-bitpixie-poc-and-winpe-edition/
* CVE-2025-22252 FortiOS 認証bypassの脆弱性
    * https://securityonline.info/fortinet-patches-critical-tacacs-authentication-bypass-cve-2025-22252-in-fortios-and-fortiproxy/
* CVE-2025-4428 Ivanti EPMM RCE
    * https://thehackernews.com/2025/05/ivanti-patches-epmm-vulnerabilities.html
    * https://securityboulevard.com/2025/05/cve-2025-4427-cve-2025-4428-ivanti-endpoint-manager-mobile-epmm-remote-code-execution/
* CVE-2025-22462 Ivanti Neurons RCE
    * https://securityonline.info/ivanti-neurons-for-itsm-hit-by-cvss-9-8-authentication-bypass-flaw-enabling-full-admin-access/
* CVE-2025-30663 Zoom 権限昇格の脆弱性
    * https://securityonline.info/zoom-patches-high-severity-flaw-cve-2025-30663-in-workplace-apps/

## KEV
* CVE-2025-30400 Microsoft Windows DWM Core Library Use-After-Free Vulnerability
* CVE-2025-32701 Microsoft Windows Common Log File System (CLFS) Driver Use-After-Free Vulnerability
* CVE-2025-32706 Microsoft Windows Common Log File System (CLFS) Driver Heap-Based Buffer Overflow Vulnerability
* CVE-2025-30397 Microsoft Windows Scripting Engine Type Confusion Vulnerability
* CVE-2025-32709 Microsoft Windows Ancillary Function Driver for WinSock Use-After-Free Vulnerability
* CVE-2025-47729 TeleMessage TM SGNL Hidden Functionality Vulnerability
    * https://www.darkreading.com/threat-intelligence/cisa-warns-telemessage-vuln-low-cvss-score
* CVE-2024-12987 DrayTek Vigor Routers OS Command Injection Vulnerability
* CVE-2025-4664 Google Chromium Loader Insufficient Policy Enforcement Vulnerability
    * https://www.securityweek.com/chrome-136-update-patches-vulnerability-with-exploit-in-the-wild/
* CVE-2025-42999 SAP NetWeaver Deserialization Vulnerability
* CVE-2025-32756 FortiMail, FortiNDR, FortiRecorder, and FortiCamera 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/fortinet-fixes-critical-zero-day-exploited-in-fortivoice-attacks/
    * https://securityonline.info/fortinet-cve-2025-32756-exploited-in-the-wild-critical-rce-flaw-hits-fortivoice-and-more/
    * https://thehackernews.com/2025/05/fortinet-patches-cve-2025-32756-zero.html

# その他
* Google Android 16 Advanced Protection によりセキュリティを強化
    * https://www.bleepingcomputer.com/news/security/android-16-expands-advanced-protection-with-device-level-security/
* Microsoft Windows10 のOfficeアプリを2028年まで更新する予定
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-will-update-office-apps-on-windows-10-until-2028/
    * https://securityonline.info/microsoft-extends-microsoft-365-support-on-windows-10-until-2028/
