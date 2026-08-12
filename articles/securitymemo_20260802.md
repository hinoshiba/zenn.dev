---
title: "2026/08/02 週 セキュリティニュースメモ"
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

* 共同通信社に不正アクセス、職員・加盟社・取引先など情報約6000件が流出のおそれ
    * https://internet.watch.impress.co.jp/docs/news/2130852.html
* 英国警察・政府関係者10万人超の個人情報流出
    * ハッカーグループExfilSquadが英国PNLDおよび政府投資機関を侵害し、警察官・政府関係者10万人超の連絡先がダークウェブに流出。政府投資部門では約40時間にわたり関係者情報が露出していた。
    * https://www.theregister.com/security/2026/08/03/uk-government-investment-arm-cops-to-40-hour-leak-of-officials-contact-details/5282213
* ロシアSVRが公衆Wi-Fiゲートウェイを乗っ取りマルウェア配布
    * https://thehackernews.com/2026/08/hijacked-hotel-wi-fi-pushes-fake.html

# 攻撃、脅威

* DOUBLECUP ClickFixサービス — ブラウザキャッシュPNG画像にマルウェアを隠蔽
    * https://www.bleepingcomputer.com/news/security/new-doublecup-clickfix-service-hides-malware-in-browser-cache-images/
* ChainDrop npmパッケージのサプライチェーン攻撃
    * https://www.bleepingcomputer.com/news/security/massive-chaindrop-npm-supply-chain-attack-infects-hundreds-of-packages/

# 脆弱性

* Atlassian Rovo AI にワンクリック脆弱性, Jira・Confluence データ漏洩の恐れ
    * https://thehackernews.com/2026/08/atlassian-rovo-can-be-tricked-into.html
* CVE-2026-64564 SCTPhantom Linux 権限昇格の脆弱性
    * https://thehackernews.com/2026/08/18-year-old-linux-sctp-flaw-could-let.html
* CVE-2026-64638 WordPress XSS2Shell xssベースの脆弱性。先月のwp2shellとは異なる
    * https://thehackernews.com/2026/08/new-wordpress-pre-auth-xss-could-lead.html

## KEV

# その他
* Claude self-hosted-runner をリリース
    * https://code.claude.com/docs/en/self-hosted-environments-quickstart
* Claude Code auto mode来週デフォルト化（8/14〜, Pro/Max/Team向け
    * https://9to5mac.com/2026/08/07/psa-claude-code-enabling-auto-mode-as-default-next-week-anthropic-says/
