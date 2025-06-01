---
title: "2025/05/04 週 セキュリティニュースメモ"
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

* PR TIMES にサイバー攻撃
    * https://www.oricon.co.jp/news/2383500/
    * https://www3.nhk.or.jp/news/html/20250508/k10014799311000.html

# 脆弱性

* CVE-2025-46762 Apache Parquet Javaの脆弱性。RCEの可能性
    * https://securityonline.info/cve-2025-46762-apache-parquet-java-flaw-allows-potential-rce-via-avro-schema/
* CVE-2025-25014 Kibana コード実行の脆弱性
    * https://securityonline.info/cve-2025-25014-cvss-9-1-prototype-pollution-in-kibana-opens-door-to-code-execution/
* CVE-2025-20188 Cisco IOS XE 任意のコード実行
    * https://www.bleepingcomputer.com/news/security/cisco-fixes-max-severity-ios-xe-flaw-letting-attackers-hijack-devices/
    * https://thehackernews.com/2025/05/cisco-patches-cve-2025-20188-100-cvss.html
    * https://securityonline.info/critical-cve-2025-20188-cvss-10-flaw-in-cisco-ios-xe-wlcs-allows-remote-root-access/
    * https://www.security-next.com/170069
    * https://www.bleepingcomputer.com/news/security/exploit-details-for-max-severity-cisco-ios-xe-flaw-now-public/
* CVE-2025-27533: Apache ActiveMQ DoS
    * https://securityonline.info/cve-2025-27533-apache-activemq-memory-allocation-bug-could-lead-to-denial-of-service/
    * https://www.exploit-db.com/exploits/52288

## KEV
* CVE-2025-27363 FreeType Out-of-Bounds Write Vulnerability
    * Android任意のコード実行の脆弱性
        * https://innovatopia.jp/cyber-security/cyber-security-news/53457/
        * https://www.bleepingcomputer.com/news/security/google-fixes-actively-exploited-freetype-flaw-on-android/
        * https://www.securityweek.com/android-update-patches-freetype-vulnerability-exploited-as-zero-day/
        * https://securityonline.info/android-security-bulletin-may-2025-multi-vulnerabilities-including-actively-exploited-cve-2025-27363/
* CVE-2025-3248 Langflow Missing Authentication Vulnerability
* CVE-2024-6047 GeoVision Devices OS Command Injection Vulnerability
    * https://securityonline.info/botnet-exploits-old-geovision-iot-devices-via-cve-2024-6047-cve-2024-11120/
* CVE-2024-11120 GeoVision Devices OS Command Injection Vulnerability
    * https://securityonline.info/botnet-exploits-old-geovision-iot-devices-via-cve-2024-6047-cve-2024-11120/


# その他
* 2025/06/05 Teamsやその他 Microsoft 365サービス障害
    * https://www.bleepingcomputer.com/news/microsoft/new-microsoft-365-outage-impacts-teams-and-other-services/
* NEC、KDDIとセキュリティ事業で協業 - 日本を守る新施設を開設へ
    * https://topics.smt.docomo.ne.jp/article/mycom/business/mycom_2974978
