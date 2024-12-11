---
title: "2024/12/01 週 セキュリティニュースメモ"
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

* LINE アルバム不具合。他人の画像が表示
    * https://www.security-next.com/164819

# 攻撃、脅威

# 脆弱性

* CVE-2024-8672 WordPress Widget Options 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-8672-critical-flaw-in-widget-options-plugin-threatens-100000-websites/
* CVE-2024-8785 Progress WhatsUp Gold RCEの脆弱性
    * https://www.bleepingcomputer.com/news/security/exploit-released-for-critical-whatsup-gold-rce-flaw-patch-now/
    * https://securityonline.info/exploit-code-available-critical-flaw-found-in-whatsup-gold-cve-2024-8785-cvss-9-8/
* CVE-2024-49039 11月のWindowsUpdateで修正されたTaskSchedulerの脆弱性。PoCリリース
    * https://securityonline.info/zero-day-exploit-code-released-for-windows-task-scheduler-flaw-cve-2024-49039-actively-exploited-by-romcom-group/
    * https://www.itmedia.co.jp/enterprise/articles/2412/05/news080.html
* CVE-2024-35368 FFmpeg ダブルフリーの脆弱性
    * https://www.security-next.com/164873
* 新しいWindowsNTLMの脆弱性。まだ公式のパッチはなし。非公式パッチあり
    * https://www.bleepingcomputer.com/news/security/new-windows-zero-day-exposes-ntlm-credentials-gets-unofficial-patch/
    * https://reinforz.co.jp/bizmedia/64761/
    * https://codebook.machinarecord.com/threatreport/36185/
    * https://www.darkreading.com/application-security/microsoft-ntlm-zero-day-remain-unpatched-april
* CVE-2024-53990 Java Library AsyncHttpClient ユーザセッションや未認証アクセスの可能性脆弱性
    * https://securityonline.info/cve-2024-53990-asynchttpclient-vulnerability-puts-java-applications-at-risk/

## KEV
* CVE-2023-45727 North Grid Proself Improper Restriction of XML External Entity (XEE) Reference Vulnerability
* CVE-2024-11680 ProjectSend Improper Authentication Vulnerability
* CVE-2024-11667 Zyxel Multiple Firewalls Path Traversal Vulnerability
* CVE-2024-51378 CyberPanel Incorrect Default Permissions Vulnerability

# その他

* マイナ保険証開始
    * https://www.ncctv.co.jp/news/article/15532145
* DMMビットコイン廃業
    * https://jp.reuters.com/markets/japan/funds/GNC6GYCUEVPFRGZYT4J7KOV4ZY-2024-12-02/
* AWS インシデントレスポンスサービスを公開
    * https://www.darkreading.com/threat-intelligence/aws-launches-new-incident-response-service
    * https://www.securityweek.com/aws-launches-incident-response-service/
* Microsoft 2025年月次アップデートの予定を公開
    * https://scan.netsecurity.ne.jp/article/2024/12/04/51991.html
* Windows 10 からWindows11へのアップグレードについて、TPM 2.0必須であることをMicrosoftが明言
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-says-having-a-tpm-is-non-negotiable-for-windows-11/
    * https://news.mynavi.jp/techplus/article/20241206-3078257/
