---
title: "2025/01/12 週 セキュリティニュースメモ"
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

* Microsoft MFAに関して障害
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-mfa-outage-blocking-access-to-microsoft-365-apps/


# 攻撃、脅威

* iPhoneユーザに対して、iMessageのフィッシング保護機能を無効化するような誘導するキャンペーン
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/iphone-users-tricked-into-disabling-apple-imessages-phishing-protection

# 脆弱性

* CVE-2025-22777 GiveWP 未認証のPHPオブジェクトインジェクションの脆弱性
    * https://securityonline.info/cve-2025-22777-cvss-9-8-critical-security-alert-for-givewp-plugin-with-100000-active-installations/
* CVE-2024-12847 NETGEAR ルータ 未認証のコマンド実行の脆弱性。PoCあり
    * https://securityonline.info/cve-2024-12847-cvss-9-8-netgear-router-flaw-exploited-in-the-wild-for-years-poc-published/
* CVE-2024-12426 LibreOffice 環境変数等の流出の可能性
    * https://forest.watch.impress.co.jp/docs/news/1653446.html
* CVE-2024-44243 昨年12月に公表されたmacOSのセキュリティ機能bypassの脆弱性、詳細レポートをMicrosoftがリリース
    * https://www.microsoft.com/en-us/security/blog/2025/01/13/analyzing-cve-2024-44243-a-macos-system-integrity-protection-bypass-through-kernel-extensions/
    * https://thehackernews.com/2025/01/microsoft-uncovers-macos-vulnerability.html
* CVE-2024-54498 昨年12月に公表されたmacOSのsandbox bypassの脆弱性、PoCリリース
    * https://securityonline.info/new-macos-exploit-revealed-poc-for-cve-2024-54498-breaks-sandbox-security/
* CVE-2025-21598 JunOS 細工されたBGPパケットによるDoS
    * https://www.securityweek.com/juniper-networks-fixes-high-severity-vulnerabilities-in-junos-os/
    * https://securityonline.info/unauthenticated-attackers-can-exploit-junos-vulnerabilities-cve-2025-21598-cve-2025-21599/
* CVE-2024-55591 FortiOS 権限昇格の脆弱性。ゼロデイ
    * https://www.bleepingcomputer.com/news/security/fortinet-warns-of-auth-bypass-zero-day-exploited-to-hijack-firewalls/
    * https://securityonline.info/active-exploitation-of-cve-2024-55591-cvss-9-6-fortios-and-fortiproxy-under-threat/
    * https://thehackernews.com/2025/01/zero-day-vulnerability-suspected-in.html
* CVE-2024-27397 Linux nftablesの権限昇格の脆弱性、PoCリリース
    * https://securityonline.info/linux-kernel-privilege-escalation-vulnerability-cve-2024-27397-exploited-poc-released/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-Jan
        * https://krebsonsecurity.com/2025/01/microsoft-happy-2025-heres-161-security-updates/
        * https://www.bleepingcomputer.com/news/microsoft/january-windows-updates-may-fail-if-citrix-sra-is-installed/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-january-2025-patch-tuesday-fixes-8-zero-days-159-flaws/

## KEV
* CVE-2024-55591 Fortinet FortiOS Authorization Bypass Vulnerability
* CVE-2025-21333 Microsoft Windows Hyper-V NT Kernel Integration VSP Heap-based Buffer Overflow Vulnerability
* CVE-2025-21334 Microsoft Windows Hyper-V NT Kernel Integration VSP Use-After-Free Vulnerability
* CVE-2025-21335 Microsoft Windows Hyper-V NT Kernel Integration VSP Use-After-Free Vulnerability
* CVE-2024-12686 BeyondTrust Privileged Remote Access (PRA) and Remote Support (RS) OS Command Injection Vulnerability
* CVE-2023-48365 Qlik Sense HTTP Tunneling Vulnerability

# その他

* 2月のWindowsUpdateにて、Windows10にOutlookがインストールされるとのこと
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-force-install-new-outlook-on-windows-10-pcs-in-february/
* LDAPNightmare に関する偽のPoCがGitHub上に設置されている。トレンドマイクロ社
    * https://www.trendmicro.com/en_us/research/25/a/information-stealer-masquerades-as-ldapnightmare-poc-exploit.html
* Officeソフトが更新後にクラッシュする不具合
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-365-apps-crash-on-windows-server-after-office-update/
