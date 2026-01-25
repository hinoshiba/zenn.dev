---
title: "2026/01/18 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、みた週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません

# 事件事故

* アプリマーケットの連携アプリ経由で顧客情報流出の可能性 - スマレジ
    * https://www.security-next.com/179645

# 攻撃、脅威

* 非公式7-Zip Webサイトにて公開されているインストーラによる不審なファイルの展開
    * https://wizsafe.iij.ad.jp/2026/01/2075/

# 脆弱性


* CVE-2026-0723 GitLab 2FA Bypass
    * https://www.bleepingcomputer.com/news/security/gitlab-warns-of-high-severity-2fa-bypass-denial-of-service-flaws/
* CVE-2026-24061 Telnetd 遠隔からの未認証リモートアクセス
    * https://seclists.org/oss-sec/2026/q1/89
    * https://www.bleepingcomputer.com/news/security/hackers-exploit-critical-telnetd-auth-bypass-flaw-to-get-root/
* Cloudflare 検査のbypass脆弱性(修正済み)
    * https://blog.cloudflare.com/acme-path-vulnerability/
    * https://www.theregister.com/2026/01/20/cloudflare_fixes_acme_validation/
    * https://thehackernews.com/2026/01/cloudflare-fixes-acme-validation-bug.html
    * https://cybersecuritynews.com/cloudflare-zero-day-vulnerability/


## KEV

# その他
* ChatGPT Go 広告付きモデルリリース
    * https://www.bleepingcomputer.com/news/artificial-intelligence/chatgpt-go-subscription-rolls-out-worldwide-at-8-but-itll-show-you-ads/
    * https://www.bleepingcomputer.com/news/artificial-intelligence/openai-says-its-new-chatgpt-ads-wont-influence-answers/
    * https://openai.com/index/introducing-chatgpt-go/
* Gmailの変更機能リリース
    * https://www.bleepingcomputer.com/news/technology/google-now-lets-you-change-your-gmailcom-address-rolling-out/
* curl AIによる不正報告が多発し、HackerOneから撤退。バグ報奨金プログラムを終了
    * https://www.bleepingcomputer.com/news/security/curl-ending-bug-bounty-program-after-flood-of-ai-slop-reports/
    * https://socket.dev/blog/curl-shuts-down-bug-bounty-program-after-flood-of-ai-slop-reports
