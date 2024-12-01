---
title: "2024/11/24 週 セキュリティニュースメモ"
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

* CVE-2024-48860 QNAP QuRouter 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-48860-cvss-9-5-critical-flaw-in-qnap-qurouter-immediate-update-recommended/
    * https://www.bleepingcomputer.com/news/security/qnap-addresses-critical-flaws-across-nas-router-software/
* CVE-2024-52899 IBM Data Virtualization Manager and Security SOAR JDBC URLパラメータによるコード実行の脆弱性
    * https://www.securityweek.com/ibm-patches-rce-vulnerabilities-in-data-virtualization-manager-security-soar/
* CVE-2024-10542 CVE-2024-10781 WordPress Plugin Anti Spam 任意のコード実行の脆弱性
    * https://thehackernews.com/2024/11/critical-wordpress-anti-spam-plugin.html
    * https://www.securityweek.com/critical-vulnerabilities-found-in-anti-spam-plugin-used-by-200000-wordpress-sites/
    * https://securityonline.info/cve-2024-10542-cve-2024-10781-critical-wordpress-plugin-flaw-exposes-200000-sites/
* CVE-2024-5921 Paloalto GlobalProtect App 悪意のあるソフトウェアがインストールされる可能性
    * https://securityonline.info/palo-alto-networks-warns-of-globalprotect-app-flaw-with-public-exploit-code-cve-2024-5921/
* CVE-2024-8932 PHP 任意のコード実行の可能性。ldap_escapeを32bit環境で利用すると影響あり
    * https://securityonline.info/php-patches-multi-flaws-including-cve-2024-8932-cvss-9-8-urges-immediate-update/
* CVE-2024-42330 Zabbix 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-42330-cvss-9-1-zabbix-patches-critical-remote-code-execution-vulnerability/
* CVE-2024-42327 Zabbix 権限昇格の脆弱性
    * https://securityonline.info/cve-2024-42327-critical-sql-injection-vulnerability-found-in-zabbix/
    * https://www.theregister.com/2024/11/29/zabbix_urges_upgrades_after_critical/

## KEV
* CVE-2023-28461 Array Networks AG and vxAG ArrayOS Missing Authentication for Critical Function Vulnerability

# その他

* Microsoft フィッシングサービスのONNX をtakedown
    * https://securityonline.info/microsoft-takes-down-onnx-phishing-as-a-service-operation/
* Cloudflare 3.5hのログ保管トラブル。55%が失われる
    * https://www.bleepingcomputer.com/news/security/cloudflare-says-it-lost-55-percent-of-logs-pushed-to-customers-for-35-hours/
    * https://securityonline.info/cloudflare-logs-suffer-critical-failure-losing-55-of-user-data/
