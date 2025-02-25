---
title: "2025/02/16 週 セキュリティニュースメモ"
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
* whoAMIというターゲットの利用しているIDから見て新しいイメージ名のAMIを用意することで、ターゲットのEC2インスタンスにロードさせる手法
    * https://thehackernews.com/2025/02/new-whoami-attack-exploits-aws-ami-name.html

# 脆弱性
* CVE-2025-1240 WinZip 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2025-1240-winzip-vulnerability-opens-door-to-remote-code-execution/
* CVE-2024-21966 AMD Ryzen Master Utility 権限昇格の脆弱性
    * https://securityonline.info/amd-ryzen-master-utility-vulnerable-to-dll-hijacking-cve-2024-21966/
* CVE-2022-31631 PHP SQLiの脆弱性
    * https://securityonline.info/cve-2022-31631-cvss-9-1-critical-php-flaw-exposes-websites-to-sql-injection-attacks/
* CVE-2025-21589 Juniper SSR 認証bypassの脆弱性
    * https://www.bleepingcomputer.com/news/security/juniper-patches-critical-auth-bypass-in-session-smart-routers/
    * https://www.securityweek.com/critical-vulnerability-patched-in-juniper-session-smart-router/
    * https://thehackernews.com/2025/02/juniper-session-smart-routers.html
    * https://securityonline.info/cve-2025-21589-cvss-9-8-critical-authentication-bypass-flaw-in-juniper-session-smart-routers/
* CVE-2025-26465 OpenSSH MITMの脆弱性
    * https://securityonline.info/openssh-flaws-cve-2025-26465-cve-2025-26466-expose-clients-and-servers-to-attacks/
    * https://www.theregister.com/2025/02/18/openssh_vulnerabilities_mitm_dos/
* 1月に修正されたLibreOfficeの脆弱性PoCリリース
    * https://securityonline.info/libreoffice-vulnerabilities-cve-2024-12425-cve-2024-12426-pocs-released-patch-asap/#google_vignette
* CVE-2024-50379 and CVE-2024-56337 Confluence Data Center and Server address RCE
    * https://www.securityweek.com/atlassian-patches-critical-vulnerabilities-in-confluence-crowd/
* CVE-2025-21420: Windows Disk Cleanup Tool 権限昇格の脆弱性
    * https://securityonline.info/cve-2025-21420-windows-disk-cleanup-tool-flaw-exploited-to-gain-system-privileges-poc-released/
* CVE-2025-26506 HP プリンタ コード実行の可能性
    * https://securityonline.info/hp-warns-of-critical-security-flaw-in-laserjet-printers-cve-2025-26506-cvssv4-9-2/

## KEV
* CVE-2025-0108 Palo Alto PAN-OS Authentication Bypass Vulnerability
* CVE-2024-53704 SonicWall SonicOS SSLVPN Improper Authentication Vulnerability
* CVE-2025-23209 Craft CMS Code Injection Vulnerability
* CVE-2025-0111 Palo Alto Networks PAN-OS File Read Vulnerability


# その他
* WSUS ドライバ同期機能停止まで、60日
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-reminds-admins-to-prepare-for-wsus-driver-sync-deprecation/
