---
title: "2026/01/04 週 セキュリティニュースメモ"
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

* スマレジ、外部アプリベンダーから会員情報漏えい
    * https://corp.smaregi.jp/news/press/20260108.php
        ```
        特定の外部アプリにおいて、外部アプリベンダーが保有する会員データが第三者によって不正に取得・公開されていた事実が判明いたしました。
        弊社サーバーにおける不審な挙動や不正アクセスの痕跡は確認されておりません
        ```
    * https://www.itmedia.co.jp/news/articles/2601/09/news095.html

# 攻撃、脅威

* BSoDを模したClickFix
    * https://www.darkreading.com/cyberattacks-data-breaches/clickfix-campaign-fake-blue-screen-of-death
    * https://thehackernews.com/2026/01/fake-booking-emails-redirect-hotel.html
    * https://www.bleepingcomputer.com/news/security/clickfix-attack-uses-fake-windows-bsod-screens-to-push-malware/
* 中国ハッカー、1日263万回侵入　情報窃取や攻撃、増加の一途　台湾
    * https://news.yahoo.co.jp/articles/136ac2fb1d9a9a505ef2bc76388d2ba9a8d502ed
    * https://www.taipeitimes.com/News/front/archives/2026/01/05/2003850052
    * https://www.nsb.gov.tw/en/#/%E5%85%AC%E5%91%8A%E8%B3%87%E8%A8%8A/%E6%96%B0%E8%81%9E%E7%A8%BF%E6%9A%A8%E6%96%B0%E8%81%9E%E5%8F%83%E8%80%83%E8%B3%87%E6%96%99/2026-01-04/Analysis%20on%20China%E2%80%99s%20Cyber%20Threats%20to%20Taiwan%E2%80%99s%20Critical%20Infrastructure%20in%202025

# 脆弱性

* CVE-2025-52835 WING WordPress Migrator CSRF
    * https://www.security-next.com/179217
    * https://nvd.nist.gov/vuln/detail/CVE-2025-52835
    * https://patchstack.com/database/wordpress/plugin/wing-migrator/vulnerability/wordpress-wing-wordpress-migrator-plugin-1-1-9-cross-site-request-forgery-csrf-vulnerability
*  CVE-2025-68668 n8n 認証済みユーザのシステムコマンド実行
    * https://thehackernews.com/2026/01/new-n8n-vulnerability-99-cvss-lets.html
*  CVE-2026-21858 n8n 未認証のコード実行
    * https://thehackernews.com/2026/01/critical-n8n-vulnerability-cvss-100.html
    * https://thehackernews.com/2026/01/n8n-warns-of-cvss-100-rce-vulnerability.html
    * https://securityonline.info/public-exploit-released-critical-n8n-flaw-cve-2026-21858-exposes-100k-servers/
* CVE-2025-69194 wget2 パストラバーサルの脆弱性
    * https://bugzilla.redhat.com/show_bug.cgi?id=2425773
* CVE-2026-20029 CISCO ISE 認証済みユーザによるコード実行の可能性。PoCあり
    * https://thehackernews.com/2026/01/cisco-patches-ise-security.html


## KEV

# その他
* CISA Known Exploited Vulnerabilities Surged 20% in 2025 @ CYBLE
    * https://cyble.com/blog/cisa-kev-2025-exploited-vulnerabilities-growth/
* アイルランドのパスポート、IRLコードに誤りがあり、1万3000まいのパスポートリコール
    * https://www.bleepingcomputer.com/news/security/ireland-recalls-almost-13-000-passports-over-missing-irl-code/
