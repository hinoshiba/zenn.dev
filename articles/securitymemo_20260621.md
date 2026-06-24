---
title: "2026/06/21 週 セキュリティニュースメモ"
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

* MoneyFoward / GitHubへの不正アクセスに関する詳細調査の完了およびセキュリティ対策強化のお知らせ（第四報）
    * https://corp.moneyforward.com/news/info/20260623-mf-press-1/
* KDDI / ISP 事業者向けメールシステムに対する不正アクセスの発生について
    * https://newsroom.kddi.com/news/assets/2026/kddi_nr_s-71_4593/kddi_nr_s-71_4593_pdf_01.pdf
* LastPass 顧客連絡先やサポート情報などの営業系データがKlue経由で流出した可能性
    * https://www.bleepingcomputer.com/news/security/lastpass-confirms-data-breach-in-klue-supply-chain-attack/
    * https://gbhackers.com/lastpass-customer-data-accessed-in-klue-supply-chain-attack/

# 攻撃、脅威

# 脆弱性

* CVE-2026-47729 Squidbleed 他セッションのHTTP平文を取得可能
    * https://thehackernews.com/2026/06/29-year-old-squid-proxy-bug-squidbleed.html
    * https://www.securityweek.com/decades-old-squid-proxy-flaw-squidbleed-can-expose-user-data/
    * https://securityonline.info/squidbleed-vulnerability/


## KEV

* CVE-2025-67038 Lantronix EDS5000 Code Injection Vulnerability
* CVE-2026-34908 Ubiquiti UniFi OS Improper Access Control Vulnerability
* CVE-2026-34909 Ubiquiti UniFi OS Path Traversal Vulnerability
* CVE-2026-34910 Ubiquiti UniFi OS Improper Input Validation Vulnerability

# その他
* GitHub actions/checkout v7をリリース。pull request target を悪用した情報窃取をブロック
    * https://gbhackers.com/github-actions-checkout-adds-protection/
    * https://thehackernews.com/2026/06/github-updates-actionscheckout-to-block.html
* OpenAI Daybreak 計画に関連するCyberモデルやプラグインを公開
    * https://openai.com/index/daybreak-securing-the-world/
