---
title: "2024/06/23 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
* あくまで、発見した週に記入します
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威
* CDK Globalsにサイバー攻撃によりサービス停止
    * https://www.darkreading.com/cloud-security/cdk-attack-contingency-planning-critical-saas-customers
    * https://www.bleepingcomputer.com/news/security/cdk-warns-threat-actors-are-calling-customers-posing-as-support/
* JAXAの不正アクセスの件が公表
    * https://cybersecurity-jp.com/news/98098
* LAの統一学区（The Los Angeles Unified School District）に関係するSnowFake上から盗まれたデータ。 hacker forumで発売される
    * https://www.bleepingcomputer.com/news/security/los-angeles-unified-confirms-student-data-stolen-in-snowflake-account-hack/
* ANYRUN フィッシング被害により電子メールが確認を受ける。本番環境への影響はないとのこと
    * https://securityonline.info/any-run-confirms-security-incident-involving-employee-email-compromise/
    * https://x.com/anyrun_app/status/1804157392935870466

# 脆弱性

* CVE-2024-5739 LINE UXSS
    * https://www.security-next.com/158827
* CVE-2024-5756: WordPress Plugin Email Subscribers SQLi
    * https://securityonline.info/cve-2024-5756-cvss-9-8-critical-icegram-express-flaw-puts-90000-wordpress-sites-at-risk/
* CVE-2024-27815: Apple 6月中旬に修正したカーネル上で任意のコードを実行できる脆弱性、PoCリリース
    * https://www.inoreader.com/article/3a9c6e740fcc85d5-cve-2024-27815-apple-xnu-kernel-vulnerability-uncovered-poc-code-released
* CVE-2024-37032: ローカルでのLLM実行OSS Ollama 任意のコード実行の脆弱性
    * https://thehackernews.com/2024/06/critical-rce-vulnerability-discovered.html
* CVE-2024-37231: WordPress Plugin Salon booking system。Pathトラバーサルの脆弱性
    * https://patchstack.com/database/vulnerability/salon-booking-system/wordpress-salon-booking-system-plugin-9-9-arbitrary-file-deletion-vulnerability
* CVE-2024-0762: Lenvo端末においてUEFI上の不具合から、バッファオーバフローの脆弱性の可能性
    * https://www.security-next.com/158794
* CVE-2024-0087: 5月に公表されたNVIDIA Tritonの脆弱性。PoCリリース
    * https://securityonline.info/poc-published-for-critical-nvidia-triton-inference-server-vulnerabilities/
* CVE-2024-2003: ESET Windows上で権限昇格の脆弱性
    * https://securityonline.info/eset-issues-security-patch-for-privilege-escalation-flaw-in-windows-products/

# その他
* MMCを利用したGrimResourceと呼ばれる新たなる攻撃手法
    * https://www.bleepingcomputer.com/news/security/new-grimresource-attack-uses-msc-files-and-windows-xss-flaw-to-breach-networks/
* シスコ、東京にサイバーセキュリティCoEを開設
    * https://news.mynavi.jp/techplus/article/20240621-2970215/
* Kasperskey製品、米国の当局で禁止措置。他
    * https://thehackernews.com/2024/06/us-bans-kaspersky-software-citing.html
    * https://www.securityweek.com/us-bans-kaspersky-software/
    * https://securityboulevard.com/2024/06/u-s-bans-sale-of-kaspersky-cybersecurity-software/
    * https://thehackernews.com/2024/06/us-treasury-sanctions-12-kaspersky.html
