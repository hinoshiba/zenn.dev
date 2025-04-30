---
title: "2025/04/27 週 セキュリティニュースメモ"
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

* 保険ショップの保険見直し本舗、個人情報510万件漏洩か
    * https://www.nikkei.com/article/DGXZQOUB304BK0Q5A430C2000000/
* 関西エアポート、1万件情報漏洩　法人向けサービス不正アクセス
    * https://www.nikkei.com/article/DGXZQOUF28AK10Y5A420C2000000/

# 脆弱性

* CVE-2025-43859 Python H11 ライブラリ Request Smugglingの脆弱性
    * https://securityonline.info/cve-2025-43859-request-smuggling-vulnerability-in-pythons-h11-http-library/
* CVE-2025-32432 Craft CMS RCE
    * https://securityonline.info/cve-2025-32432-cvss-10-craft-cms-hit-by-critical-rce-flaw-exploited-in-the-wild/
    * https://securityonline.info/craft-cms-zero-day-cve-2025-32432-exploited-with-metasploit-module-now-public/
* CVE-2025-31324 SAP NetWeaver 任意の操作が可能。C2として利用されるゼロデイ
    * https://securityonline.info/cve-2025-31324-cvss-10-zero-day-in-sap-netweaver-exploited-in-the-wild-to-deploy-webshells-and-c2-frameworks/
    * https://www.securityweek.com/sap-zero-day-possibly-exploited-by-initial-access-broker/
    * https://www.theregister.com/2025/04/25/sap_netweaver_patch/
    * https://securityonline.info/cisa-adds-sap-netweaver-zero-day-cve-2025-31324-to-kev-database/
* CVE-2025-31650 Apache Tomcat DoSの脆弱性
    * https://rocket-boys.co.jp/security-measures-lab/apache-tomcat-cve-2025-31650-dos-security-bypass-risk/
    * https://securityonline.info/apache-tomcat-security-update-fixes-dos-and-rewrite-rule-bypass-flaws/
* CVE-2025-24252、CVE-2025-24132 AirBorne という攻撃手法。AirPlay経由によりRCEの可能性
    * https://www.bleepingcomputer.com/news/security/apple-airborne-flaws-can-lead-to-zero-click-airplay-rce-attacks/
    * https://www.securityweek.com/airplay-vulnerabilities-expose-apple-devices-to-zero-click-takeover/
    * https://securityonline.info/airborne-exploits-zero-click-wormable-rce-hits-apple-iot-devices/
* CVE-2025-42598 セイコーエプソンプリンタドライバにより権限昇格の可能性
    * https://www.security-next.com/169884
* CVE-2024-22031 Rancher 権限昇格の脆弱性
    * https://securityonline.info/rancher-releases-patch-for-cve-2024-22031-privilege-escalation-vulnerability/

## KEV
* CVE-2025-1976 Broadcom Brocade Fabric OS Code Injection Vulnerability
* CVE-2025-42599 Qualitia Active! Mail Stack-Based Buffer Overflow Vulnerability
* CVE-2025-3928 Commvault Web Server Unspecified Vulnerability
* CVE-2025-31324 SAP NetWeaver Unrestricted File Upload Vulnerability

# その他


