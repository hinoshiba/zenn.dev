---
title: "2025/10/05 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見たニュースである事に留意ください

# 事件事故

* Discord、外部業者への不正アクセスで情報流出　運転免許証やパスポートも
    * https://news.yahoo.co.jp/articles/1eb1bbab2d92452fe3658e8fcfc0b9fb75cf002f
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/discord-users-data-stolen-by-hackers-in-third-party-data-breach
    * https://databreaches.net/2025/10/09/discord-confirms-70000-government-ids-exposed-in-third-party-breach/

# 攻撃、脅威

* セキュリティ更新を装ったfilefix
    * https://www.bleepingcomputer.com/news/security/new-filefix-attack-uses-cache-smuggling-to-evade-security-software/
* 楽天証券 リアルタイムフィッシング
    * https://japan.cnet.com/article/35239128/
* ランサムウェア「Qilin」を操る攻撃者グループ「Water Galura」とは？～2022年頃から活動するランサムウェア攻撃者グループ
    * https://www.trendmicro.com/ja_jp/jp-security/25/j/securitytrend-20251010-01.html

# 脆弱性

* CVE-2025-61882 Oracle E-Business Suite RCE
    * https://dailydarkweb.net/oracle-patches-cve%E2%88%922025%E2%88%9261882/
    * https://www.theregister.com/2025/10/06/clop_oracle_ebs_zeroday/
    * https://www.securityweek.com/oracle-e-business-suite-zero-day-exploited-in-cl0p-attacks/
    * https://thehackernews.com/2025/10/oracle-rushes-patch-for-cve-2025-61882.html
    * https://www.bleepingcomputer.com/news/security/oracle-patches-ebs-zero-day-exploited-in-clop-data-theft-attacks/
* CVE-2025-10728 Qt DoS
    * https://securityonline.info/qt-fixes-dual-critical-vulnerabilities-cve-2025-10728-cve-2025-10729-in-svg-module/
* CVE-2025-49844 Redis RCE
    * https://www.bleepingcomputer.com/news/security/redis-warns-of-max-severity-flaw-impacting-thousands-of-instances/
    * https://securityboulevard.com/2025/10/redis-lua-code-execution-vulnerability-cve-2025-49844-notice/
* CVE-2025-27915 メールクライアント、Zimbra iscファイルを用いたXSS
    * https://www.bleepingcomputer.com/news/security/hackers-exploited-zimbra-flaw-as-zero-day-using-icalendar-files/
* CVE-2025-59978 Junos XSS
    * https://www.securityweek.com/juniper-networks-patches-critical-junos-space-vulnerabilities/


## KEV
* CVE-2025-27915 Synacor Zimbra Collaboration Suite (ZCS) Cross-site Scripting Vulnerability
* CVE-2010-3765 Mozilla Multiple Products Remote Code Execution Vulnerability
* CVE-2010-3962 Microsoft Internet Explorer Uninitialized Memory Corruption Vulnerability
* CVE-2011-3402 Microsoft Windows Remote Code Execution Vulnerability
* CVE-2013-3918 Microsoft Windows Out-of-Bounds Write Vulnerability
* CVE-2021-22555 Linux Kernel Heap Out-of-Bounds Write Vulnerability
* CVE-2021-43226 Microsoft Windows Privilege Escalation Vulnerability
* CVE-2025-61882 Oracle E-Business Suite Unspecified Vulnerability 
* CVE-2021-43798 Grafana Path Traversal Vulnerability

# その他
* Windows 11 23H2 来月EoS
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-23h2-home-and-pro-reach-end-of-support-in-30-days/
