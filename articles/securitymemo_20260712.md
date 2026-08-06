---
title: "2026/07/12 週 セキュリティニュースメモ"
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

* ニチレイ
    * 当社グループでのシステム障害発生について
        * https://www.nichirei.co.jp/news/2026/512.html
        * https://www.nichirei.co.jp/news/2026/513.html
        * https://www.nichirei.co.jp/news/2026/514.html
    * 物流委託先のシステム障害に伴う一部店舗の営業への影響について(7月18日更新) / KFC
        * https://japan.kfc.co.jp/news_release/8160

# 攻撃、脅威
* 新型macOSマルウェアClickLock Stealerが210ms間隔でアプリを強制終了し、ユーザーにパスワード再入力を強制してシステムパスワードを窃取する。macOSのセキュリティ機構をソーシャルエンジニアリングで回避。
    * https://thehackernews.com/2026/07/new-clicklock-macos-stealer-kills-apps.html

# 脆弱性

* Windows Update 7月
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-jul
    * https://thehackernews.com/2026/07/microsoft-patches-record-622-flaws.html
    * https://www.theregister.com/security/2026/07/14/patchpocalypse-now-microsoft-tops-last-months-record-with-622-patch-tuesday-cves/5271434
    * Dell PC でパフォーマンスの低下やバッテリーの著しい消費、シャットダウンの問題があり、一時停止
        * https://www.theregister.com/os-platforms/2026/07/15/microsoft-cancels-patch-tuesday-for-some-dell-users-over-surprise-shutdowns-overheating-devices/5271691
        * https://gbhackers.com/microsoft-blocks-windows-11-security-update-on-dell/
* CVE-2026-63030 and CVE-2026-60137 wp2shell
    * https://thehackernews.com/2026/07/new-wp2shell-wordpress-core-flaw-lets.html
    * https://securityboulevard.com/2026/07/imperva-customers-protected-against-wp2shell-pre-authentication-rce-in-wordpress-core/
* HollowByte OpenSSL DoS 11バイのデータにより。
    * https://thehackernews.com/2026/07/openssl-hollowbyte-flaw-could-freeze.html


## KEV

* CVE-2026-25089 Fortinet FortiSandbox OS Command Injection Vulnerability  
    * https://www.theregister.com/security/2026/07/17/attackers-target-critical-fortisandbox-flaws-as-cisa-issues-patch-order/5274287
* CVE-2026-39808 Fortinet FortiSandbox OS Command Injection Vulnerability  
* CVE-2026-58644 Microsoft SharePoint Deserialization of Untrusted Data Vulnerability
    * https://thehackernews.com/2026/07/cisa-adds-exploited-sharepoint-rce-zero.html

# その他
* GPT-Red発表 — 自己対戦型自動レッドチーミングシステム、プロンプトインジェクション防御を自動強化
    * https://openai.com/index/unlocking-self-improvement-gpt-red
* Telegram t[.]meドメイン 一時停止
    * https://gbhackers.com/telegrams-t-me-domain-suspended/
* Fable 5 提供継続
    https://the-decoder.com/anthropic-slashes-claude-fable-5-limits-in-max-and-team-premium-and-pushes-pro-users-toward-api-pricing/
    * https://securityonline.info/claude-fable-5-subscription-changes/
