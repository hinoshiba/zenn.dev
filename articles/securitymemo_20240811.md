---
title: "2024/08/11 週 セキュリティニュースメモ"
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

* CVE-2024-38200 MicrosoftOfficeを通じて、NTLMハッシュを窃取する脆弱性。機能アップデートで配布済み。最終盤は、8月のWindowsUpdateで配布予定
    * https://www.bleepingcomputer.com/news/security/microsoft-discloses-unpatched-office-flaw-that-exposes-ntlm-hashes/
    * https://securityonline.info/cve-2024-38200-zero-day-vulnerability-in-microsoft-office-a-call-for-urgent-action/
* CVE-2024-7589 FreeBSD 系のOpenSSH 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-7589-openssh-pre-authentication-vulnerability-in-freebsd-exposes-systems-to-rce/
    * https://thehackernews.com/2024/08/freebsd-releases-urgent-patch-for-high.html
    * https://www.security-next.com/160746
* CVE-2024-6768 Windows 11/10 CLFSによるBSoD
    * https://www.darkreading.com/vulnerabilities-threats/clfs-bug-crashes-even-updated-windows-10-11-systems
* Microsoft研究者、OpenVPNに対する脆弱性を用いた攻撃チェーンにて、RCEのデモを実施。BlachHat 2024にて
    * https://www.microsoft.com/en-us/security/blog/2024/08/08/chained-for-attack-openvpn-vulnerabilities-discovered-leading-to-rce-and-lpe/
    * https://www.securityweek.com/microsoft-warns-of-openvpn-vulnerabilities-potential-for-exploit-chains/
    * https://news.mynavi.jp/techplus/article/20240813-3004164/
* CVE-2024-34117 Adobe Photoshop コード実行
    * https://www.securityweek.com/adobe-calls-attention-to-massive-batch-of-code-execution-flaws/
* CVE-2024-7569 and CVE-2024-7570 Ivanti ITSM 未認証のアクセスの脆弱性
    * https://securityonline.info/ivanti-issues-critical-fixes-for-itsm-vulnerabilities-cve-2024-7569-and-cve-2024-7570/
* CVE-2024-7593 Ivanti Virtual Traffic Manager (vTM)、認証bypassの脆弱性。PoCあり
    * https://www.bleepingcomputer.com/news/security/ivanti-warns-of-critical-vtm-auth-bypass-with-public-exploit/
    * https://securityonline.info/cve-2024-7593-cvss-9-8-authentication-bypass-in-ivanti-vtm-proof-of-concept-available/
* CVE-2024-39825 Zoom 権限昇格の脆弱性
    * https://securityonline.info/cve-2024-39825-and-cve-2024-39818-high-risk-zoom-flaws-require-urgent-updates/
* CVE-2024-22116 Zabbix 認証済みユーザによる任意のコード実行
    * https://securityonline.info/zabbix-addresses-multi-vulnerabilities-including-rce-cve-2024-36461-cvss-9-1-flaw/
    * https://securityonline.info/cve-2024-22116-cvss-9-9-critical-rce-vulnerability-found-in-zabbix-monitoring-solution/
    * https://support.zabbix.com/browse/ZBX-25016
    * https://www.security-next.com/160763
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Aug
        * https://www.tripwire.com/state-of-security/vert-threat-alert-august-2024-patch-tuesday-analysis
        * https://krebsonsecurity.com/2024/08/six-0-days-lead-microsofts-august-2024-patch-push/
        * https://www.darkreading.com/vulnerabilities-threats/microsoft-discloses-10-zero-day-bugs-in-pacth-tuesday-update
        * https://www.securityweek.com/microsoft-warns-of-six-windows-zero-days-being-actively-exploited/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-august-2024-patch-tuesday-fixes-9-zero-days-6-exploited/
        * https://www.cisa.gov/news-events/alerts/2024/08/13/microsoft-releases-august-2024-security-updates
        * https://www.security-next.com/160776
        * M365 Defender WindowsServerにおいてネットワーク保護機能が壊れている不具合、8月のアップデートで修正
            * https://www.bleepingcomputer.com/news/microsoft/windows-server-august-updates-fix-microsoft-365-defender-issue/
    * cve
        * Publicly Discosed
            * CVE-2024-21302 Windows Secure Kernel Mode Elevation of Privilege Vulnerability
            * CVE-2024-38199 Windows Line Printer Daemon (LPD) Service Remote Code Execution Vulnerability
        * Exploited
            * CVE-2024-38189 Microsoft Project Remote Code Execution Vulnerability
            * CVE-2024-38107 Windows Power Dependency Coordinator Elevation of Privilege Vulnerability
            * CVE-2024-38106 Windows Kernel Elevation of Privilege Vulnerability
            * CVE-2024-38213 Windows Mark of the Web Security Feature Bypass Vulnerability
                * https://www.bleepingcomputer.com/news/microsoft/new-windows-smartscreen-bypass-exploited-as-zero-day-since-march/
            * CVE-2024-38193 Windows Ancillary Function Driver for WinSock Elevation of Privilege Vulnerability
            * CVE-2024-38178 Scripting Engine Memory Corruption Vulnerability
        * その他
            * CVE-2024-38173 Microsoft Outlook Remote Code Execution Vulnerability
                * プレビューペインでも発火
            * CVE-2024-38171 Microsoft PowerPoint Remote Code Execution Vulnerabilit
                * プレビューペインでも発火
* KEV
    * CVE-2024-38189 Microsoft Project Remote Code Execution Vulnerability
    * CVE-2024-38107 Microsoft Windows Power Dependency Coordinator Privilege Escalation Vulnerability
    * CVE-2024-38106 Microsoft Windows Kernel Privilege Escalation Vulnerability
    * CVE-2024-38213 Microsoft Windows SmartScreen Security Feature Bypass Vulnerability
    * CVE-2024-38193 Microsoft Windows Ancillary Function Driver for WinSock Privilege Escalation Vulnerability
    * CVE-2024-38178 Microsoft Windows Scripting Engine Memory Corruption Vulnerability

# その他

* Windows 11 22H2 EOSまであと60日。(2024/10/08迄)
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-11-22h2-reaches-end-of-support-in-60-days/
* Microsoft Paint 3D 今年11月に削除予定とのこと
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-is-killing-the-windows-paint-3d-app-after-8-years/
* Google ロシアへの広告支払いの最後を実施
    * https://www.bleepingcomputer.com/news/google/google-deactivates-russian-adsense-accounts-sends-final-payments/
* NIST Post-Quantum暗号標準を最終決定
    * https://www.darkreading.com/endpoint-security/nist-finalizes-post-quantum-encryption-standards
    * https://securityboulevard.com/2024/08/nist-announces-the-first-3-post-quantum-cryptography-standards-ready-or-not/
* FBI Radar/Dispossessor ランサムウェアサーバを停止
    * https://www.darkreading.com/cyberattacks-data-breaches/fbi-shuts-down-dozens-of-radar-dispossessor-ransomware-servers
    * https://thehackernews.com/2024/08/fbi-shuts-down-dispossessor-ransomware.html
    * https://www.securityweek.com/radar-dispossessor-ransomware-operation-disrupted-by-authorities/
* Windows 11 8月アップデート新機能まとめ
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-kb5041585-cumulative-update-released-with-fixes-new-features/
* Google Cloudサービス、2時間以上停止。イギリス
    * https://securityonline.info/google-cloud-services-disrupted-in-uk-due-to-power-outage/
