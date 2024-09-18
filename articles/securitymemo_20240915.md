---
title: "2024/09/15 週 セキュリティニュースメモ"
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

* CVE-2024-28991 SolarWinds Access Rights Manager (ARM) 任意のコード実行
    * https://www.securityweek.com/solarwinds-patches-critical-vulnerability-in-access-rights-manager/
    * https://thehackernews.com/2024/09/solarwinds-issues-patch-for-critical.html
* iOS 17.7 更新
    * https://forest.watch.impress.co.jp/docs/news/1624053.html
* CVE-2024-38812 VMware vCenter Server 任意のコード実行
    * https://www.theregister.com/2024/09/17/vmware_vcenter_patch/
    * https://www.bleepingcomputer.com/news/security/broadcom-fixes-critical-rce-bug-in-vmware-vcenter-server/
    * https://www.securityweek.com/vmware-patches-remote-code-execution-flaw-found-in-chinese-hacking-contest/
* CVE-2024-6091 AutoGPT OS Command Injection
    * https://securityonline.info/166k-projects-at-risk-autogpts-critical-vulnerability-explained-cve-2024-6091-cvss-9-8/
* KEV
    * CVE-2024-43461 MSHTML RCE
        * https://www.darkreading.com/application-security/void-banshee-exploits-second-microsoft-zero-day
        * https://www.bleepingcomputer.com/news/security/cisa-warns-of-windows-flaw-used-in-infostealer-malware-attacks/
        * https://securityonline.info/new-zero-day-emerges-after-microsoft-patch-tuesday-cve-2024-43461-targets-windows-mshtml/
        * https://www.bleepingcomputer.com/news/security/windows-vulnerability-abused-braille-spaces-in-zero-day-attacks/
    * CVE-2024-6670 Progress WhatsUp Gold SQL Injection Vulnerability
    * CVE-2014-0497 Adobe Flash Player Integer Underflow Vulnerability
    * CVE-2013-0643 Adobe Flash Player Incorrect Default Permissions Vulnerability
    * CVE-2013-0648 Adobe Flash Player Code Execution Vulnerability
    * CVE-2014-0502 Adobe Flash Player Double Free Vulnerability

# その他

* Microsoft 365 appに対してスペルチェックによるクラッシュの不具合を修正
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-bug-crashing-microsoft-365-apps-when-typing/
* Microsoft Office LTSC 2024 ロールアウト
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-rolls-out-office-ltsc-2024-for-windows-and-mac/
* Apple iOS 18をリリース
    * https://forest.watch.impress.co.jp/docs/news/1624051.html
    * https://www.securityweek.com/apple-patches-major-security-flaws-with-ios-18-refresh/
* Apple Passwords アプリをリリース
    * https://securityboulevard.com/2024/09/apples-new-passwords-app-a-game-changer-for-user-security-and-the-cybersecurity-landscape/
* Cloudflareいくつかのリージョンで障害か？ 2024/09/17 1:45 PM ET
    * https://www.bleepingcomputer.com/news/technology/cloudflare-outage-cuts-off-access-to-websites-in-some-regions/
* 1,000以上のServiceNowのユーザがKB程度のデータを漏洩している可能性が見つかった
    * https://www.bleepingcomputer.com/news/security/over-1-000-servicenow-instances-found-leaking-corporate-kb-data/
    * https://securityboulevard.com/2024/09/enterprise-servicenow-knowledge-bases-at-risk-extensive-data-exposures-uncovered/
