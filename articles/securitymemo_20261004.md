---
title: "2026/10/04 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。

# 事件事故

* 日本経済新聞社の社員アカウントにサイバー攻撃、取引先・取材先へなりすましメール約9000件を不正送信
    * https://www.nikkei.com/article/DGXZQOUD255YG0V20C26A9000000/
* 大阪公立大学でランサムウェア攻撃、約500台のサーバー停止・全授業休講、学生ら約13万人分の個人情報流出の恐れ
    * https://piyolog.hatenadiary.jp/entry/2026/10/07/095650
* 『焼肉きんぐ』公式アプリ 会員管理システムへの第三者からの不正アクセスによる個人情報漏えいに関するお詫び
    * https://www.monogatari.co.jp/news/261005_news/
* 大和証券 委託先の問い合わせ管理サービスへの不正アクセスで約11万人の顧客情報が漏えいした可能性
    * https://ssl4.eir-parts.net/doc/8601/tdnet/2891437/00.pdf
* GMO 当社が運営するアンケートサイト「infoQ」への不正アクセスによる個人情報漏えいに関するお詫びとお知らせ
    * https://gmo-research.ai/pressroom/notice/notice-20261005
* 「楽天ドライブ」における不正アクセスの発生について
    * https://support.rakuten-drive.com/hc/ja/articles/62934949147929--%E9%87%8D%E8%A6%81-%E6%A5%BD%E5%A4%A9%E3%83%89%E3%83%A9%E3%82%A4%E3%83%96-%E3%81%AB%E3%81%8A%E3%81%91%E3%82%8B%E4%B8%8D%E6%AD%A3%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%81%AE%E7%99%BA%E7%94%9F%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6
* 「ローソンID」システムに不正アクセス、会員アプリ関連の個人情報215万件超が流出
    * https://www.lawson.co.jp/contents/cont07/1533174_3310.html
* 西鉄のICカード「nimoca」利用履歴照会サービスに不正アクセス、521件の情報が漏えい
    * https://news.web.nhk/newsweb/na/nd-20261006de55188
* ブックオフ会員管理システムへの不正アクセス、最大643万件の会員情報が漏えいのおそれ
    * https://news.web.nhk/newsweb/na/nd-20261009de56955

# 攻撃、脅威

* .gh・.sl・.asのレジストリが乗っ取られ、Google等のドメイン向け偽証明書が発行される
    * https://thehackernews.com/2026/10/attackers-hijack-gh-sl-and-as.html

# 脆弱性

* AWS Bedrock AgentCoreの欠陥、単一プロンプトでAIエージェントを乗っ取り可能に
    * https://www.theregister.com/security/2026/10/09/aws-agentcore-security-undone-by-prompt-requesting-credentials/5302436


# その他
* OpenAI、EU向けChatGPT・Codexテキストに不可視透かし「textGrain」を導入
    * https://openai.com/index/eu-text-provenance/
* SpaceXAI、「SpaceXSI」へ改称へ。Trump大統領が9/29の大統領令で、連邦機関にAIを「超知能(SI)」と呼ぶよう指示したことを受けた動き
    * https://thenextweb.com/news/musk-spacexai-renamed-spacexsi
* JR, Suicaコード決済、Teppay の開始 10/20
    * https://prtimes.jp/main/html/rd/p/000001542.000017557.html
* Google オープンソース向けバグ報奨金プログラム一時停止
    * https://www.bleepingcomputer.com/news/google/google-halts-open-source-bug-bounty-program-amid-ai-spam-surge/
* Anthoropic Cyber Verification Programを拡張、3段階のアクセス階層を新設
    * https://www.anthropic.com/news/cyber-verification-program
* Anthropic、OSSプロジェクト向けの無償AI脆弱性スキャナー「OSS Scanner」を発表
    * https://thehackernews.com/2026/10/anthropic-launches-free-ai.html
* Google Cloud、汎用の職場向け「Gemini agent」を発表
    * https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/gemini-at-work/
