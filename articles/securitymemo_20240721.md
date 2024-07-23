---
title: "2024/07/21 週 セキュリティニュースメモ"
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

* Crowdstrike Falconの世界的な不具合、修正ツールをMicrosoftが配布
    * https://techcommunity.microsoft.com/t5/intune-customer-success/new-recovery-tool-to-help-with-crowdstrike-issue-impacting/ba-p/4196959
    * https://www.securityweek.com/microsoft-says-8-5-million-windows-devices-impacted-by-crowdstrike-incident-publishes-recovery-tool/
    * https://securityboulevard.com/2024/07/new-microsoft-recovery-tool-for-crowdstrike-issue-on-windows-endpoints/

# 攻撃、脅威

* Crowdstrike FalconによるBSoDに関連する、マルウェア配布キャンペーン
    * https://thehackernews.com/2024/07/cybercriminals-exploit-crowdstrike.html
    * https://www.bleepingcomputer.com/news/security/fake-crowdstrike-fixes-target-companies-with-malware-data-wipers/
    * https://www.crowdstrike.com/blog/likely-ecrime-actor-capitalizing-on-falcon-sensor-issues/

# 脆弱性
* CVE-2024-20416 Cisco RV340などに対する任意のコード実行
    * https://securityonline.info/cisco-warns-of-unpatched-vulnerability-cve-2024-20416-in-rv340-and-rv345-routers/
* CVE-2024-36455 Symantec PAM 任意のコード実行の脆弱性
    * https://securityonline.info/broadcom-urges-immediate-patching-for-critical-symantec-pam-vulnerabilities/
* CVE-2024-38437 D-Link 認証bypassの脆弱性
    * https://cvefeed.io/vuln/detail/CVE-2024-38437
* Telegram アンドロイドアプリケーション上で、悪意のあるヴィデオのより、APKファイルのインストールを促す脆弱性
    * https://securityonline.info/evilvideo-vulnerability-zero-day-threat-targets-telegram-for-android/
    * https://www.bleepingcomputer.com/news/security/telegram-zero-day-allowed-sending-malicious-android-apks-as-videos/

# その他

* Google 2025年8月にショートURLサービス`goo.gl`のサポートを終了。以降は、404になる予定
    * https://securityonline.info/google-url-shortener-ends-support-what-you-need-to-know-before-august-2025/
    * https://developers.googleblog.com/en/google-url-shortener-links-will-no-longer-be-available/
* Google サードパーティ製Cookieのblockを撤回
    * https://www.bleepingcomputer.com/news/security/google-rolls-back-decision-to-kill-third-party-cookies-in-chrome/
* Thunderbird システムトレイ通知対応
    * https://www.theregister.com/2024/07/22/mozilla_thunderbird_ffix/
* DigitalStressをテイクダウン。NCA主導
    * https://www.bleepingcomputer.com/news/security/police-infiltrates-takes-down-digitalstress-ddos-for-hire-service/
* ソフトウェア等の脆弱性関連情報に関する届出状況[2024年第2四半期（4月～6月）]
    * https://www.ipa.go.jp/security/reports/vuln/software/2024q2.html
    * https://www.security-next.com/159975
