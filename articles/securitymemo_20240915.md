---
title: "2024/09/15 週 セキュリティニュースメモ"
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

* シンガポール子会社にサイバー攻撃、他関連会社に影響なし - ヤマトHD
    * https://www.security-next.com/161892
* Disney サイバー攻撃を受けSlackの利用を禁止へ
    * https://www.msn.com/ja-jp/money/other/%E3%83%87%E3%82%A3%E3%82%BA%E3%83%8B%E3%83%BC-%E3%82%B9%E3%83%A9%E3%83%83%E3%82%AF-%E4%BD%BF%E7%94%A8%E4%B8%AD%E6%AD%A2%E3%81%B8-%E3%82%B5%E3%82%A4%E3%83%90%E3%83%BC%E6%94%BB%E6%92%83%E3%81%A7%E6%83%85%E5%A0%B1%E6%B5%81%E5%87%BA/ar-AA1qRy0V
    * https://www.theregister.com/2024/09/20/disney_slack_microsoft_teams/
    * https://gigazine.net/news/20240920-disney-to-stop-using-slack/
* レバノンの無線機機爆発について、icom社からニュースリリース
    * https://www.icom.co.jp/news/8110/
* 大樹生命、最大７万人分の顧客情報流出か
    * https://www.topics.or.jp/articles/-/1130490
* Dell 10,000名以上の従業員のデータがハッキングにより流出
    * https://www.bleepingcomputer.com/news/security/dell-investigates-data-breach-claims-after-hacker-leaks-employee-info/

# 脆弱性

* CVE-2024-28991 SolarWinds Access Rights Manager (ARM) 任意のコード実行
    * https://www.securityweek.com/solarwinds-patches-critical-vulnerability-in-access-rights-manager/
    * https://thehackernews.com/2024/09/solarwinds-issues-patch-for-critical.html
* iOS 17.7 更新
    * https://forest.watch.impress.co.jp/docs/news/1624053.html
* CVE-2024-38812 VMware vCenter Server 任意のコード実行
    * https://www.theregister.com/2024/09/17/vmware_vcenter_patch/
    * https://www.bleepingcomputer.com/news/security/broadcom-fixes-critical-rce-bug-in-vmware-vcenter-server/
    * https://www.securityweek.com/vmware-patches-remote-code-execution-flaw-found-in-chinese-hacking-contest/
    * https://thehackernews.com/2024/09/patch-issued-for-critical-vmware.html
* CVE-2024-6091 AutoGPT OS Command Injection
    * https://securityonline.info/166k-projects-at-risk-autogpts-critical-vulnerability-explained-cve-2024-6091-cvss-9-8/
* CVE-2024-8904 Google Chrome 任意のコード実行の可能性
    * https://www.securityweek.com/chrome-129-patches-high-severity-vulnerability-in-v8-engine/
* CVE-2024-7788 LibreOffice 署名偽装の脆弱性
    * https://securityonline.info/libreoffice-vulnerability-cve-2024-7788-exploit-of-repair-mode-signatures-raises-security-concerns/
* CVE-2024-38014 9月のWindowsUpdateで修正されたMSIインストーラによるゼロデイ、詳細解説
    * https://securityonline.info/researchers-detail-cve-2024-38014-0-day-vulnerability-in-windows-msi-installers-exploited-in-the-wild/
* KEV
    * CVE-2024-43461 MSHTML RCE
        * https://www.darkreading.com/application-security/void-banshee-exploits-second-microsoft-zero-day
        * https://www.bleepingcomputer.com/news/security/cisa-warns-of-windows-flaw-used-in-infostealer-malware-attacks/
        * https://securityonline.info/new-zero-day-emerges-after-microsoft-patch-tuesday-cve-2024-43461-targets-windows-mshtml/
        * https://www.bleepingcomputer.com/news/security/windows-vulnerability-abused-braille-spaces-in-zero-day-attacks/
    * CVE-2024-6670 Progress WhatsUp Gold SQL Injection Vulnerability
    * CVE-2014-0497 Adobe Flash Player Integer Underflow Vulnerability
        * https://www.security-next.com/161957
    * CVE-2013-0643 Adobe Flash Player Incorrect Default Permissions Vulnerability
    * CVE-2013-0648 Adobe Flash Player Code Execution Vulnerability
    * CVE-2014-0502 Adobe Flash Player Double Free Vulnerability
    * CVE-2024-27348 Apache HugeGraph-Server Improper Access Control Vulnerability
        * https://www.bleepingcomputer.com/news/security/cisa-warns-of-actively-exploited-apache-hugegraph-server-bug/
    * CVE-2020-0618 Microsoft SQL Server Reporting Services Remote Code Execution Vulnerability
    * CVE-2019-1069 Microsoft Windows Task Scheduler Privilege Escalation Vulnerability
    * CVE-2022-21445 Oracle JDeveloper Remote Code Execution Vulnerability
    * CVE-2020-14644 Oracle WebLogic Server Remote Code Execution Vulnerability
    * CVE-2024-8963 Ivanti Cloud Services Appliance (CSA) Path Traversal Vulnerability
        * https://www.bleepingcomputer.com/news/security/ivanti-warns-of-another-critical-csa-flaw-exploited-in-attacks/

# その他

* Microsoft 365 appに対してスペルチェックによるクラッシュの不具合を修正
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-bug-crashing-microsoft-365-apps-when-typing/
* Microsoft Office LTSC 2024 ロールアウト
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-rolls-out-office-ltsc-2024-for-windows-and-mac/
* Apple iOS 18をリリース
    * https://forest.watch.impress.co.jp/docs/news/1624051.html
    * https://www.securityweek.com/apple-patches-major-security-flaws-with-ios-18-refresh/
* Apple Passwords アプリをリリース
    * https://securityboulevard.com/2024/09/apples-new-passwords-app-a-game-changer-for-user-security-and-the-cybersecurity-landscape/
* Cloudflareいくつかのリージョンで障害か？ 2024/09/17 1:45 PM ET
    * https://www.bleepingcomputer.com/news/technology/cloudflare-outage-cuts-off-access-to-websites-in-some-regions/
* 1,000以上のServiceNowのユーザがKB程度のデータを漏洩している可能性が見つかった
    * https://www.bleepingcomputer.com/news/security/over-1-000-servicenow-instances-found-leaking-corporate-kb-data/
    * https://securityboulevard.com/2024/09/enterprise-servicenow-knowledge-bases-at-risk-extensive-data-exposures-uncovered/
    * https://www.darkreading.com/cloud-security/servicenow-kb-instances-expose-corporate-data
* Discord 音声通話やビデオ通話のエンドツーエンド暗号をリリース
    * https://www.bleepingcomputer.com/news/security/discord-rolls-out-end-to-end-encryption-for-audio-video-calls/
* アメリカ、パスポートの申請をオンラインで可能に
    * https://jp.reuters.com/life/3QOHJSNQI5NVJOCLCVCYBMZROA-2024-09-18/
* Windows 24H2 順次リリース
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-may-have-revealed-windows-11-24h2-is-coming-this-month/
* Excel Python提供開始。特定ユーザに限る
    * https://www.theregister.com/2024/09/18/python_in_excel_general_release/
* Google Passwordマネージャ、パスキーの保存と端末間の自動同期に対応
    * https://www.bleepingcomputer.com/news/google/google-password-manager-now-automatically-syncs-your-passkeys/
    * https://thehackernews.com/2024/09/chrome-users-can-now-sync-passkeys.html
    * https://news.mynavi.jp/techplus/article/20240920-3028945/
* WSUS 将来的に提供を終了。クラウド管理への移行が推奨
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-officially-deprecates-windows-server-update-services-wsus/
* Windows Server 2025 ホットパッチ対応
    * https://www.bleepingcomputer.com/news/microsoft/windows-server-2025-hotpatching-in-public-preview-installs-security-updates-without-restarts/
* ウクライナ、安全保障上の理由により国支給の端末によるテレグラムアプリの利用を禁止
    * https://www.securityweek.com/ukraine-bans-telegram-messenger-app-on-state-issued-devices-because-of-russian-security-threat/
    * https://www.bleepingcomputer.com/news/security/ukraine-bans-telegram-on-military-govt-devices-over-security-risks/
