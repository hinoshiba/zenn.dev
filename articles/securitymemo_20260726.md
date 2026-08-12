---
title: "2026/07/26 週 セキュリティニュースメモ"
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

* Claudeの共有チャット・Artifactsがsite:claude.ai/shareでGoogle検索可能な状態になっていたことが発覚, 7/27時点でインデックス削除はほぼ完了
    * https://venturebeat.com/technology/uh-oh-some-claude-shared-conversations-and-artifacts-appear-to-be-indexed-and-publicly-accessible-on-google-search
* ミネソタ州30以上の水道システムへの協調的OTサイバー攻撃
    * https://www.theregister.com/security/2026/07/29/iran-linked-cyberav3ngers-suspected-in-attacks-on-minnesota-water-systems/5280357
# 攻撃、脅威
* Cruciferra Crypter, BYOVD+プロセスゴースティングでEDR回避
    * https://thehackernews.com/2026/07/cruciferra-crypter-uses-byovd-and.html
* Joyfill npm パッケージ侵害, RAT・資格情報窃取
    * https://socket.dev/blog/joyfill-npm-beta-releases-compromised
* Microsoft Copilot for Wordワーム, 隠しプロンプトが自動伝播
    * https://www.theregister.com/security/2026/07/29/word-worm-crawls-into-copilot-spreads-chaos/5280588
* Anthropic Claudeがテストサンドボックスを脱出し3組織を攻撃
    * https://www.theregister.com/ai-and-ml/2026/07/31/anthropics-claude-escaped-test-sandbox-to-attack-three-organizations/5281562


# 脆弱性

* CVE-2026-66066 Ruby on Rails Active Storageに重大なRCE脆弱性
    * https://thehackernews.com/2026/07/critical-rails-flaw-could-let.html
    * https://blog.flatt.tech/entry/kindarails2shell_rails


## KEV

# その他
* GitHub/PyPI サプライチェーン防御ポリシー強化
    * https://thehackernews.com/2026/07/github-adds-3-day-dependabot-cooldown.html
* 米国が外国製ヒューマノイドロボットを禁止
    * https://www.theregister.com/security/2026/07/29/america-bans-imported-robots-due-to-supply-chain-and-security-risks/5280145
* Revolut、OpenAIと提携しChatGPT Goを顧客に提供
    * https://www.revolut.com/news/revolut-partners-with-openai-to-bring-chatgpt-go-to-millions-of-customers/
