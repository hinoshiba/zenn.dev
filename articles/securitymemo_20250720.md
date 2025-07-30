---
title: "2025/07/20 週 セキュリティニュースメモ"
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

* 総務省がIIJに行政指導、Active! mailの脆弱性による顧客情報漏洩で
    * https://xtech.nikkei.com/atcl/nxt/news/24/02704/
* DELL テスト環境のデータが盗まれる。WoldLeaksが関与か。
    * https://www.bleepingcomputer.com/news/security/dell-confirms-breach-of-test-lab-platform-by-world-leaks-extortion-group/


# 攻撃、脅威

* SNSパトロールから逮捕　遠隔操作ウイルス販売目的所持で25歳男を逮捕　京都府警
    * https://news.jp/i/1319225295220605737?c=768367547562557440
* BlackSuitリークサイト、takedown
    * https://www.bleepingcomputer.com/news/security/law-enforcement-seizes-blacksuit-ransomware-leak-sites/


# 脆弱性

* CVE-2025-4700 GitLab XSS k8s proxy上で。
    * https://securityonline.info/gitlab-update-high-severity-xss-data-exposure-flaws-patched/
* CVE-2025-8069 AWS VPN CLient 権限昇格の脆弱性
    * https://securityonline.info/high-severity-flaw-cve-2025-8069-in-aws-client-vpn-for-windows-allows-privilege-escalation/

## KEV
* CVE-2025-53770 ToolShell Sharepoint 他脆弱性と組み合わせることで未認証のRCE。ゼロデイ
    * https://www.darkreading.com/remote-workforce/microsoft-rushes-emergency-fix-exploited-sharepoint-toolshell-flaw
    * https://securityboulevard.com/2025/07/hackers-exploiting-microsoft-flaw-to-attack-governments-businesses/
    * https://www.securityweek.com/microsoft-patches-toolshell-zero-days-exploited-to-hack-sharepoint-servers/
    * https://www.theregister.com/2025/07/21/infosec_in_brief/
    * https://securityonline.info/metasploit-module-released-for-actively-exploited-microsoft-sharepoint-flaw-cve-2025-53770/
    * https://securityonline.info/microsoft-china-backed-apts-actively-exploiting-sharepoint-flaws-cve-2025-49704-cve-2025-49706/
    * https://www.securityweek.com/microsoft-says-chinese-apts-exploited-toolshell-zero-days-weeks-before-patch/
    * CVE-2025-49704 Microsoft SharePoint Code Injection Vulnerability
    * CVE-2025-49706 Microsoft SharePoint Improper Authentication Vulnerability
    * https://scan.netsecurity.ne.jp/article/2025/07/25/53290.html
* CVE-2025-54309 CrushFTP Unprotected Alternate Channel Vulnerability
* CVE-2025-6558 Google Chromium ANGLE and GPU Improper Input Validation Vulnerability
* CVE-2025-2776 SysAid On-Prem Improper Restriction of XML External Entity Reference Vulnerability
* CVE-2025-2775 SysAid On-Prem Improper Restriction of XML External Entity Reference Vulnerability


# その他
* Micorosft 365 管理画面障害
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-investigates-outage-affecting-microsoft-365-admin-center/
