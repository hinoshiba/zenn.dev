---
title: "2026/11/15 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。

# 事件事故

* 京成電鉄「スカイライナー」の座席予約システムに不正アクセス、最大約337万件の顧客情報が流出の可能性
    * https://www.nikkei.com/article/DGXZQOUC13CBJ0T11C26A1000000/
* ヤマダデンキのリフォーム管理システムに不正アクセス、最大約350万件の顧客情報が漏えいのおそれ
    * https://news.web.nhk/newsweb/na/nd-20261113de75739
* Uber、委託先の認証情報悪用で約15万人のドライバーの運転免許証画像・個人情報が流出
    * https://www.securityweek.com/uber-data-breach-impacts-150000-people/
* 楽天証券のテスト環境に不正アクセス、最大約1125万口座のログインID等と最大約447万口座の年収・資産情報などが漏えいのおそれ
    * https://news.yahoo.co.jp/articles/141fe69b0f33952604cde710494bbdff584f269a

# 攻撃、脅威

* Google GTIG、攻撃者がAIエージェントでパッチ差分から攻撃コードを自動生成・実行する事例を初確認 — 「完全自律型の攻撃は6か月以内に出現」と予測
    * https://cloud.google.com/blog/topics/threat-intelligence/agentic-threat-activity-crosses-a-significant-threshold
* A/Bテスト基盤「Optimizely」経由のサプライチェーン攻撃、CNN・BBC・Zoomなど178組織のサイトに暗号資産を盗むマルウェアが配信
    * https://coinpost.jp/?p=748196

# 脆弱性

* CVE-2026-99288 Linux Kernel リモートからのクラッシュ。NoisyTCP
    * https://access.redhat.com/security/cve/cve-2026-99288


# その他
* Anthropic、AIが見つけた脆弱性の公開までの期間を90日から30日・45日に短縮
    * https://red.anthropic.com/research/coordinated-vulnerability-disclosure-timelines
* GPT-6.2 Astra / GPT-6.2 Solを公開
    * https://openai.com/index/introducing-gpt-6-2-astra-sol/
