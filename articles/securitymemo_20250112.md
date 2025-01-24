---
title: "2025/01/12 週 セキュリティニュースメモ"
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

* Microsoft MFAに関して障害
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-mfa-outage-blocking-access-to-microsoft-365-apps/

# 攻撃、脅威

* iPhoneユーザに対して、iMessageのフィッシング保護機能を無効化するような誘導するキャンペーン
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/iphone-users-tricked-into-disabling-apple-imessages-phishing-protection
* Google検索結果に表示されるGoogle広告の管理ページに対して、偽のページへ誘導する広告ページを作成する攻撃キャンペーン
    * https://www.bleepingcomputer.com/news/security/hackers-use-google-search-ads-to-steal-google-ads-accounts/

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
    * https://www.securityweek.com/fortinet-confirms-new-zero-day-exploitation/
    * https://scan.netsecurity.ne.jp/article/2025/01/17/52173.html
    * https://securityboulevard.com/2025/01/fortinet-os-fortiproxy-authentication-bypass-vulnerability-cve-2024-55591-notification/
* CVE-2023-37936 FortiSwitch コード実行の脆弱性
    * https://securityonline.info/cve-2023-37936-cvss-9-6-urgent-patch-needed-for-fortiswitch-vulnerability/
* CVE-2024-27397 Linux nftablesの権限昇格の脆弱性、PoCリリース
    * https://securityonline.info/linux-kernel-privilege-escalation-vulnerability-cve-2024-27397-exploited-poc-released/
* CVE-2024-12084 rsync コード実行の可能性を含む脆弱性の公開
    * https://thehackernews.com/2025/01/google-cloud-researchers-uncover-flaws.html
    * https://securityonline.info/cve-2024-12084-cvss-9-8-code-execution-risk-rsync-vulnerability-demands-immediate-patching/
    * https://news.mynavi.jp/techplus/article/20250117-3108101/
    * QNAP 更新
        * https://www.bleepingcomputer.com/news/security/qnap-fixes-six-rsync-vulnerabilities-in-hbs-nas-backup-recovery-app/
* CVE-2025-0147 Zoom Linux環境においてネットワーク経由の権限昇格の脆弱性
    * https://securityonline.info/cve-2025-0147-zoom-fixes-high-severity-security-flaw/
* CVE-2025-0107 PaloAlto OSコマンド実行の脆弱性。PoCあり
    * https://securityonline.info/cve-2025-0107-poc-exploit-code-released-for-palo-alto-expedition-rce-flaw/
* CVE-2024-53691 QNAP RCEの脆弱性、PoCリリース
    * https://securityonline.info/cve-2024-53691-poc-exploit-released-for-severe-qnap-rce-flaw/
* CVE-2025-23013 Yubico pam-u2f 権限昇格の脆弱性
    * https://securityonline.info/yubico-addresses-authentication-bypass-vulnerability-cve-2025-23013-in-pam-u2f-package/
* CVE-2025-0282 Iavnti Connect Secure 他 未認証の接続などの脆弱性。PoCあり
    * https://securityonline.info/poc-exploit-released-for-ivanti-connect-secure-flaw-cve-2025-0282-used-in-attacks/
* CVE-2024-9042 k8s Windowsのnode上で任意のコード事項の脆弱性
    * https://securityonline.info/cve-2024-9042-code-execution-vulnerability-found-in-kubernetes-windows-nodes/
* CVE-2024-12365 W3 Total Cache 未認証のアクセス、SSRFの脆弱性
    * https://securityonline.info/cve-2024-12365-popular-wordpress-caching-plugin-exposes-millions-of-sites-to-attack/
    * https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/w3-total-cache/w3-total-cache-281-authenticated-subscriber-missing-authorization-to-server-side-request-forgery
    * https://www.bleepingcomputer.com/news/security/w3-total-cache-plugin-flaw-exposes-1-million-wordpress-sites-to-attacks/
    * https://rocket-boys.co.jp/12079/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-Jan
        * https://krebsonsecurity.com/2025/01/microsoft-happy-2025-heres-161-security-updates/
        * https://www.bleepingcomputer.com/news/microsoft/january-windows-updates-may-fail-if-citrix-sra-is-installed/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-january-2025-patch-tuesday-fixes-8-zero-days-159-flaws/
        * https://securityboulevard.com/2025/01/microsofts-january-security-update-of-high-risk-vulnerabilities-in-multiple-products/
        * CVE-2025-21298 Outlook ゼロクリック脆弱性
            * https://securityonline.info/microsoft-patches-outlook-zero-click-cve-2025-21298-exploits-rce-via-emails/

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
* Google OAuthに関して、第三者がアカウントを取得しなおすことで、サービスへサインインが可能となる問題への報告
    * https://www.msn.com/ja-jp/news/techandscience/google%E3%81%A7%E3%82%B5%E3%82%A4%E3%83%B3%E3%82%A4%E3%83%B3-%E3%81%AE%E9%87%8D%E5%A4%A7%E3%81%AA%E8%84%86%E5%BC%B1%E6%80%A7%E3%81%8C%E6%8C%87%E6%91%98%E3%81%95%E3%82%8C%E3%82%8B/ar-AA1xe3h1
    * https://trufflesecurity.com/blog/millions-at-risk-due-to-google-s-oauth-flaw
* Windows 11 管理者プロテクト機能をプレビューばんへ追加。管理者でログインしていても常時は標準ユーザとして動作し、ソフトウェアインストール等でPINや生体認証によって認証する
    * https://www.bleepingcomputer.com/news/security/microsoft-expands-testing-of-windows-11-admin-protection-feature/
* Windows 11無償アップグレードには期限あり、早めに対応を
    * https://news.mynavi.jp/techplus/article/20250116-3107920/
* Microsoft Edgeのpdfリーダ、Acrobatに移行。2025年半ば
    * https://www.windowslatest.com/2025/01/13/microsoft-edge-could-soon-load-pdf-faster-on-windows-11-especially-low-end-pcs/
* Microsoft Windows 11 22H2, 23H3の強制アップグレードを開始
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-starts-force-upgrading-windows-11-22h2-23h3-devices/
