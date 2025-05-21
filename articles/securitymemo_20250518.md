---
title: "2025/05/18 週 セキュリティニュースメモ"
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

* コインベース 70Kの顧客情報流出
    * https://www.darkreading.com/threat-intelligence/coinbase-breach-compromises-70k-customers
    * https://www.coinbase.com/en-gb/blog/protecting-our-customers-standing-up-to-extortionists

# 攻撃、脅威

# 脆弱性

* CVE-2025-4802 glibc コード実行の可能性
    * https://securityonline.info/glibc-vulnerability-cve-2025-4802-puts-millions-of-linux-systems-at-risk-of-code-execution/
* CVE-2025-4918 FireFox 領域外メモリ書き込み
    * https://www.bleepingcomputer.com/news/security/mozilla-fixes-firefox-zero-days-exploited-at-hacking-contest/
    * https://thehackernews.com/2025/05/firefox-patches-2-zero-days-exploited.html
    * https://securityonline.info/pwn2own-firefox-hacked-with-javascript-zero-days-details-on-the-exploits/
* CVE-2025-22157  Jira Service Management Data Center and Server 権限昇格の脆弱性
    * https://securityonline.info/high-severity-privilege-escalation-threat-hits-atlassian-jira-data-center/
* CVE-2025-41227 VMware ESXi, Workstation, and Fusion DoSの脆弱性
    * https://www.cvedetails.com/cve/CVE-2025-41227/
    * https://securityonline.info/broadcom-fixes-rce-dos-xss-in-vmware-esxi-vcenter-workstation/
* CVE-2025-41232 Spring Framework 未認証のアクセスの可能性
    * https://securityonline.info/spring-framework-flaw-allows-unauthorized-access-via-security-bypass/
* CVE-2025-40775 BIND DDoS
    * https://www.cvedetails.com/cve/CVE-2025-40775/
    * https://securityonline.info/bind-dns-server-vulnerable-to-remote-crash/
* CVE-2025-47934 OpenPGP.js 署名検証のbypassの脆弱性
    * https://www.security-next.com/170544

## KEV

* CVE-2025-4427 Ivanti Endpoint Manager Mobile (EPMM) Authentication Bypass Vulnerability
* CVE-2025-4428 Ivanti Endpoint Manager Mobile (EPMM) Code Injection Vulnerability
* CVE-2024-11182 MDaemon Email Server Cross-Site Scripting (XSS) Vulnerability
* CVE-2025-27920 Srimax Output Messenger Directory Traversal Vulnerability
* CVE-2024-27443 Synacor Zimbra Collaboration Suite (ZCS) Cross-Site Scripting (XSS) Vulnerability
* CVE-2023-38950 ZKTeco BioTime Path Traversal Vulnerability

# その他
* WSL OSS化
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-open-sources-windows-subsystem-for-linux-at-build-2025/
    * https://securityonline.info/wsl-goes-open-source-microsoft-opens-up-windows-subsystem-for-linux/
