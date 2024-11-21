---
title: "2024/11/10 週 セキュリティニュースメモ"
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
* CVE-2024-47295 SEIKO EPSON のデバイス、管理者権限を容易に乗っ取られる脆弱性
    * https://securityonline.info/unpatched-epson-devices-at-risk-cve-2024-47295-allows-easy-hijacking/
* CVE-2024-50330 Ivanti Endpoint Manager RCE
    * https://securityonline.info/cve-2024-50330-cvss-9-8-unpatched-ivanti-endpoint-manager-vulnerable-to-rce-attacks/
* CVE-2024-47574 Fortinet VPN Client 高い権限で任意の実行を第三者に行われる可能性
    * https://www.theregister.com/2024/11/14/fortinet_vpn_authentication_bypass_bug/
* CVE-2024-9693 GitLab Kubernetes Agent 未認証のアクセスの可能性
    * https://securityonline.info/cve-2024-9693-gitlab-issues-critical-patch-for-kubernetes-agent/
    * https://www.security-next.com/164207
* CVE-2024-11120 GeoVision 未認証のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/botnet-exploits-geovision-zero-day-to-install-mirai-malware/
    * https://securityonline.info/cve-2024-11120-os-command-injection-flaw-in-geovision-devices-actively-exploited-no-patch/
* CVE-2024-0012 Paloalto 未認証のコード実行の脆弱性。PoCあり
    * https://www.bleepingcomputer.com/news/security/palo-alto-networks-warns-of-potential-pan-os-rce-vulnerability/
    * https://www.bleepingcomputer.com/news/security/palo-alto-networks-warns-of-critical-rce-zero-day-exploited-in-attacks/
    * https://www.securityweek.com/palo-alto-networks-confirms-new-firewall-zero-day-exploitation/
    * https://thehackernews.com/2024/11/pan-os-firewall-vulnerability-under.html
    * https://www.bleepingcomputer.com/news/security/palo-alto-networks-patches-two-firewall-zero-days-used-in-attacks/
    * https://securityonline.info/cve-2024-0012-and-cve-2024-9474-actively-exploited-vulnerabilities-impact-palo-alto-networks-pan-os/
    * https://www.security-next.com/164355
    * https://securityonline.info/analysis-poc-exploits-released-for-palo-alto-zero-days-cve-2024-0012-and-cve-2024-9474/
* CVE-2024-10979 PostgreSQL 任意のコード実行や情報漏洩の可能性
    * https://thehackernews.com/2024/11/high-severity-flaw-in-postgresql-allows.html
* CVE-2024-52301 Laravel 未認証のアクセスや権限昇格の可能性
    * https://securityonline.info/critical-laravel-flaw-cve-2024-52301-exposes-millions-of-web-applications-to-attack/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Nov
        * https://securityboulevard.com/2024/11/patch-tuesday-update-november-2024/
        * https://www.darkreading.com/cloud-security/2-zero-day-bugs-microsoft-nov-update-active-exploit
        * https://krebsonsecurity.com/2024/11/microsoft-patch-tuesday-november-2024-edition/
        * https://www.securityweek.com/microsoft-confirms-zero-day-exploitation-of-task-scheduler-flaw/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-november-2024-patch-tuesday-fixes-4-zero-days-91-flaws/
    * news
        * https://www.bleepingcomputer.com/news/security/microsoft-patches-windows-zero-day-exploited-in-attacks-on-ukraine/
## KEV
* CVE-2021-26086 Atlassian Jira Server and Data Center Path Traversal Vulnerability
* CVE-2014-2120 Cisco Adaptive Security Appliance (ASA) Cross-Site Scripting (XSS) Vulnerability
* CVE-2021-41277 Metabase GeoJSON API Local File Inclusion Vulnerability
* CVE-2024-43451 Microsoft Windows NTLMv2 Hash Disclosure Spoofing Vulnerability
* CVE-2024-49039 Microsoft Windows Task Scheduler Privilege Escalation Vulnerability
* CVE-2024-9463 Palo Alto Networks Expedition OS Command Injection Vulnerability
* CVE-2024-9465 Palo Alto Networks Expedition SQL Injection Vulnerability

# その他
* Windows 11 22H2 and 23H2 10月のWindowsUpdate以降SSHの接続に失敗する不具合がある。ワークアラウンドあり
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-says-recent-windows-11-updates-break-ssh-connections/
* iPhone 長時間の放置時に自動再起動することで、再暗号化し、デバイスのセキュリティを高める機能を追加
    * https://www.bleepingcomputer.com/news/security/iphones-now-auto-restart-to-block-access-to-encrypted-data-after-long-idle-times/
* WindowsServer2025への勝手にアップグレードした問題、サードパーティ製品の更新管理システムの影響か
    * https://learn.microsoft.com/en-us/windows/release-health/status-windows-server-2025#3404msgdesc
* Windows 11 Arm版、直接ISOのDLが可能に
    * https://www.theregister.com/2024/11/14/windows_11_arm_iso/
* Broadcom VMWare Workstation ProおよびFusionを無償化へ
    * https://blogs.vmware.com/cloud-foundation/2024/11/11/vmware-fusion-and-workstation-are-now-free-for-all-users/
    * https://www.theregister.com/2024/11/14/vmware_workstation_free/
    * https://news.mynavi.jp/techplus/article/20241113-3063120/
* Microsoft Windwos 10 ベータチャンネルをクローズ
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-just-killed-the-windows-10-beta-channel-for-good/
    * https://news.mynavi.jp/techplus/article/20241115-3065337/
