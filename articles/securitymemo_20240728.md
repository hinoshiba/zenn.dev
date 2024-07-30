---
title: "2024/07/28 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威
* Google WorkSpaceの認証機能を用い第三者のアカウントを奪い取る不具合を修正。悪用試みがあり
    * https://securityonline.info/google-patches-workspace-authentication-flaw-thwarting-account-takeover-attempts/
* シャープ、公式EC「COCORO STORE｣で不正アクセス　203件の個人情報流出
    * https://www.watch.impress.co.jp/docs/news/1612161.html
    * https://news.google.com/rss/articles/CBMiKmh0dHBzOi8vc3AubS5qaWppLmNvbS9hcnRpY2xlL3Nob3cvMzI5ODAwOdIBAA?oc=5&hl=en-US&gl=US&ceid=US:en

# 脆弱性

* CVE-2024-5285 WP Affiliate Platform 情報削除 CSRF
    * https://wpscan.com/vulnerability/792f3904-88bd-47d1-9049-afccdd74853a/
* OAuthの実装不備によるXSSの脆弱性。HotJar and Business Insider を例にSalt Labsが報告
    * https://www.securityweek.com/millions-of-websites-susceptible-xss-attack-via-oauth-implementation-flaw/
    * https://salt.security/blog/over-1-million-websites-are-at-risk-of-sensitive-information-leakage---xss-is-dead-long-live-xss
    * https://www.darkreading.com/endpoint-security/oauth-xss-attack-millions-web-users-account-takeover
* KEV
    * CVE-2024-4879 ServiceNow Improper Input Validation Vulnerability
    * CVE-2024-5217 ServiceNow Incomplete List of Disallowed Inputs Vulnerability
    * CVE-2023-45249 Acronis Cyber Infrastructure (ACI) Insecure Default Password Vulnerability

# その他

* Windows11 タスクバーから、タスクの終了が選べるように。デフォルトだと無効
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-taskbar-has-a-hidden-end-task-feature-how-to-turn-it-on/
* X(Twitter) LLMsのトレーニングを開始。オプトアウト手順あり
    * https://www.bleepingcomputer.com/news/security/x-begins-training-grok-ai-with-your-posts-heres-how-to-disable/
    * https://securityonline.info/x-formerly-twitter-silently-trains-ai-on-user-data-sparks-privacy-concerns/
* iOS 18.1 ベータ 公開によりAppleIntelligenceのテスト利用が可能
    * https://www.bleepingcomputer.com/news/apple/apple-ios-181-beta-previews-apple-intelligence-for-the-first-time/
* 投資ファンド・日本サイバーセキュリティファンド（NCSF）は7月29日、新たに出資者として参加するセキュリティ企業13社を発表
    * https://www.itmedia.co.jp/news/articles/2407/29/news150.html
* PKfail。UEFIセキュアブートのプラットフォームキーがGitHub上に上がっていた。暗号化されていたが４文字パスワードだった
    * https://www.theregister.com/2024/07/29/infosec_roundup/
    * https://www.binarly.io/blog/pkfail-untrusted-platform-keys-undermine-secure-boot-on-uefi-ecosystem
    * https://gigazine.net/news/20240726-pkfail/
