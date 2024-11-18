---
title: "2024/11/17 週 セキュリティニュースメモ"
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

* 2024/11/15 Salesforce 大規模障害
    * https://status.salesforce.com/incidents/13457
    * https://piyolog.hatenadiary.jp/entry/2024/11/18/040039

# 攻撃、脅威

# 脆弱性
* CVE-2024-38812 and CVE-2024-38813 脆弱性公表からパッチ適用まで1ヶ月ほど。すでに攻撃に利用されているため、パッチの適用を呼びかけ
    * https://www.bleepingcomputer.com/news/security/critical-rce-bug-in-vmware-vcenter-server-now-exploited-in-attacks/
    * https://www.theregister.com/2024/11/18/vmware_vcenter_rce_exploited/
* CVE-2024-10924 WordPress Plugin Really Simple Security(SSL) 認証bypassの脆弱性
    * https://thehackernews.com/2024/11/urgent-critical-wordpress-plugin.html
    * https://rocket-boys.co.jp/10663/

## KEV
* CVE-2024-1212 Progress Kemp LoadMaster OS Command Injection Vulnerability
* CVE-2024-0012 Palo Alto Networks PAN-OS Management Interface Authentication Bypass Vulnerability
* CVE-2024-9474 Palo Alto Networks PAN-OS Management Interface OS Command Injection Vulnerability


# その他

* Brave iOS版、Wipe機能が追加
    * https://www.bleepingcomputer.com/news/security/brave-on-ios-adds-new-shred-button-to-wipe-site-specific-data/