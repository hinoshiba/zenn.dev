---
title: "2026/11/08 週 セキュリティニュースメモ"
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

* ニトリ、不正アクセスにより個人・法人会員の情報最大3762万件が流出の可能性
    * https://internet.watch.impress.co.jp/docs/news/2154931.html
* 「ラクスル」に不正アクセス印刷データ漏えいか
    * https://news.tv-asahi.co.jp/news_economy/articles/000546354.html
* 早稲田大、PHP脆弱性への対応中に不正アクセス発見　個人情報約3400件流出確認
    * https://www.itmedia.co.jp/news/article/2611/09/2000003012/
* Iris Ohyamaのオンラインストア「アイリスプラザ」でクラウド経由の情報漏えい、最大770万人分
    * https://www.bleepingcomputer.com/news/security/iris-ohyama-data-cloud-breach-exposes-info-of-77-million-customers/
* Fireworks AIが2度目の侵害を公表、クラウド事業者経由で顧客データセット・未完成モデル重み・Notion AIのチャットが露出
    * https://fireworks.ai/security/bulletins/october-2026-security-incident-update
* SMBC日興証券の持株会管理システムに不正アクセス、会員最大5万6487人分の個人情報が漏えい
    * https://www.bloomberg.com/jp/news/articles/2026-11-11/TOBIOVKK3NYB00?srnd=jp-homepage#gsc.tab=0
* セキュリティ企業サイバーセキュリティクラウドの開発用GitHubに不正アクセス、従業員の認証情報流出で顧客情報漏えいのおそれ
    * https://www.cscloud.co.jp/news/info/20261112-2/

# 攻撃、脅威
* Microsoftの研究者、10個未満のニューロン編集でAIエージェント用モデルにバックドアを仕込む手法「Lazarus」を発表
    * https://www.microsoft.com/en-us/security/blog/2026/11/10/detecting-sleeper-agents-hiding-in-ai-model-neurons/

# 脆弱性
* Windows Update 11月
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-Nov
* Windows CLFSのログ認証機能を悪用してSYSTEM権限を得るゼロデイ「SignDrop」のPoCが公開、修正・CVEなし
    * https://thehackernews.com/2026/11/new-signdrop-zero-day-exploit-turns.html
* CVE-2026-119618 Apache mod_http2 RCEの脆弱性
    * https://httpd.apache.org/security/vulnerabilities_24.html#CVE-2026-119618


# その他
* Claude Fable 5.2 / Mythos 5.2を公開
    * https://www.anthropic.com/claude-fable-and-mythos-5-2
* Businesses in ChatGPT(ベータ)を公開
    * https://openai.com/index/introducing-businesses-chatgpt/
* OpenAIが、ショッピングエージェント「dots」が代わりに購入まで行うための決済機能ChatGPT Walletを公開
    * https://openai.com/index/introducing-chatgpt-wallet/
* Microsoft 365で世界規模の障害、Outlook・Teams・Copilot・Defender XDRなどが長時間利用不能に
    * https://www.bleepingcomputer.com/news/microsoft/massive-microsoft-365-outage-disrupts-outlook-teams-copilot-worldwide/
