---
title: "2026/11/22 週 セキュリティニュースメモ"
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

* EU欧州委員会に大規模サイバー攻撃、職員の個人情報流出の可能性・AIエージェント悪用か
    * https://www.asahi.com/articles/ASVCM4DWLVCMUHBI02YM.html
* JAXAの地球観測データ公開システムに不正アクセス、利用者2000人分のアカウント情報が流出
    * https://www.asahi.com/articles/ASVCS2CC8VCSUTFL00PM.html
* 日本マクドナルド、公式アプリのデータベースに不正アクセス
* MJS M&Aパートナーズの社内ネットワークへの不正アクセス
    * https://utm.hinoshiba.com/2026/11/mjs-ma-partners-unauthorized-access/
* ENEOS公式アプリへの不正アクセス
    * https://utm.hinoshiba.com/2026/11/eneos-app-unauthorized-access/

# 攻撃、脅威

# 脆弱性

* CVE-2026-131914 開発終了したASP.NETのCSRF対策ライブラリ「Idunno.AntiCsrf」に認証不要のRCE脆弱性 CVSS 9.3 / 悪用を確認
    * https://github.com/mandiant/Vulnerability-Disclosures/blob/master/2026/MNDT-2026-0048.md
* CVE-2026-133325 Apache Tomcatに認証回避の脆弱性 TLS 1.3＋TLS-PSKのクラスタ通信で未認証ノードが参加可能
    * https://access.redhat.com/security/cve/cve-2026-133325


# その他
* OpenAIとCisco、未修正のLinuxをパッチ適用まで守るオープンソースの防御ツール「Shirudo」を公開 — AIエージェントがeBPFの「シールド」を作成し再起動なしで悪用経路を遮断
    * https://openai.com/index/introducing-shirudo/
* Cloudflare、AIエージェントがサイト内を検索できる「Search for Agents」をベータ公開
    * https://blog.cloudflare.com/search-for-agents/
