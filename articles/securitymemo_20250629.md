---
title: "2025/06/29 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
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

* Qantas航空、サイバー攻撃。600万人の顧客情報盗難を発表
    * https://www.bleepingcomputer.com/news/security/qantas-discloses-cyberattack-amid-scattered-spider-aviation-breaches/
    * https://databreaches.net/2025/07/01/qantas-customers-involved-in-mammoth-data-breach/
    * https://www.theregister.com/2025/07/02/qantas_data_theft/
    * https://www.bleepingcomputer.com/news/security/qantas-is-being-extorted-in-recent-data-theft-cyberattack/
* 米国、北朝鮮IT労働者スキームの仲介者を逮捕
    * https://www.theregister.com/2025/06/30/us_north_korea_workers/
    * https://thehackernews.com/2025/07/us-arrests-key-facilitator-in-north.html
* 旧アトレカード券面記載のQRコード到達のドメイン、第三者に取得される
    * https://www.atre.co.jp/news/5360/
* ClickFixのフォルダエクスプローラ実行を促すFileFix
    * https://www.darkreading.com/endpoint-security/clickfix-spin-off-bypassing-key-browser-safeguards
* 追加の再発防止策発表 ～ PR TIMES への不正アクセス
    * https://www.excite.co.jp/news/article/Scannetsecurity_53162/
* ポケモンセンターオンラインで情報漏えいか、不正ログイン確認　約9日の緊急メンテ経てサービス再開
    * https://www.itmedia.co.jp/news/articles/2507/03/news073.html


# 脆弱性

* CVE-2025-32463 Linux 権限昇格。Sudo -R により。
    * https://securityonline.info/critical-sudo-flaws-cve-2025-32463-cvss-9-3-root-privilege-escalation-host-bypass-poc-available/
    * https://thehackernews.com/2025/07/critical-sudo-vulnerabilities-let-local.html
* CVE-2025-20309 Cisco Unified CM RCE
    * https://securityonline.info/cve-2025-20309-cvss-10-cisco-patches-critical-static-ssh-root-credential-flaw-in-unified-cm/

## KEV
* CVE-2025-48927 TeleMessage TM SGNL Initialization of a Resource with an Insecure Default Vulnerability
* CVE-2025-48928 TeleMessage TM SGNL Exposure of Core Dump File to an Unauthorized Control Sphere Vulnerability
* CVE-2025-6543 Citrix NetScaler ADC and Gateway Buffer Overflow Vulnerability
* CVE-2025-6554 Google Chromium V8 Type Confusion Vulnerability


# その他

* Cloudflare AIによるスキャンをデフォルトブロック。7/1から。
    * https://www.securityweek.com/cloudflare-puts-a-default-block-on-ai-web-scraping/
* Microsoft Authenticator パスワードマネージャ機能を8/1に終了
    * https://thehackernews.com/2025/07/microsoft-removes-password-management.html
* Windows 11のシェア、ついにWindows 10に追いつく
    * https://news.mynavi.jp/techplus/article/20250702-3369103/
* Powershell 2.0 そろそろ削除
    * https://www.theregister.com/2025/07/04/microsoft_finally_bids_farewell_to/
* 【第10回】情報セキュリティ事故対応アワード
    * https://news.mynavi.jp/techplus/article/20250704-3368463/
