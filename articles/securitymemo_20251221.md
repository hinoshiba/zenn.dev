---
title: "2025/12/21 週 セキュリティニュースメモ"
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

# 攻撃、脅威
* VPN 拡張機能、Phantom Shuttle、認証情報を含めて送信していたという報告
    * https://socket.dev/blog/malicious-chrome-extensions-phantom-shuttle

# 脆弱性

* CVE-2025-68615 Net-SNMP DoS
    * https://github.com/net-snmp/net-snmp/security/advisories/GHSA-4389-rwqf-q9gq
* CVE-2025-14847 MongoDB 未認証のデータ読み込み
    * https://thehackernews.com/2025/12/new-mongodb-flaw-lets-unauthenticated.html
    * https://www.bleepingcomputer.com/news/security/exploited-mongobleed-flaw-leaks-mongodb-secrets-87k-servers-exposed/


## KEV

# その他
* Docker Hardened Images(DHI) 無料化
    * https://www.bleepingcomputer.com/news/security/docker-hardened-images-now-open-source-and-available-for-free/
* Gmail、メールアドレスのユーザ部分変更可能へ
    * https://www.bleepingcomputer.com/news/google/google-will-finally-allow-you-to-change-your-gmailcom-address/
    * https://support.google.com/accounts/answer/19870?dark=0&sjid=9364014948975224882-NC&hl=ja
