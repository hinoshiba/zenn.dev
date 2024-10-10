---
title: "2024/10/06 週 セキュリティニュースメモ"
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
* 東京損保鑑定 ランサムウェア被害。東京海上日動火災保険と損害保険ジャパン、三井住友海上火災保険。東京海上日動「ランサムウェア」で委託先の約7.2万件の情報漏えいか
    * https://article.auone.jp/detail/1/3/6/333_6_r_20241007_1728299659331319 
    * https://article.auone.jp/detail/1/3/6/16_6_r_20241007_1728296191809527 
* インターネットアーカイブ ハッキングを受ける.
    * https://www.bleepingcomputer.com/news/security/internet-archive-hacked-data-breach-impacts-31-million-users/
    * https://haveibeenpwned.com/PwnedWebsites#InternetArchive
    * https://codebook.machinarecord.com/threatreport/35074/
    * https://securityboulevard.com/2024/10/internet-archive-is-attacked-and-31-million-files-stolen/
* Casio ネットワーク侵害により製品リリースが遅れる
    * https://securityonline.info/casio-confirms-network-breach-investigates-potential-data-compromise/

# 脆弱性
* CVE-2024-30052 Visual Studio ダンプファイルを用いた任意のコード実行の脆弱性
    * https://gbhackers.com/cve-2024-30052-visual-studio-exploit/  
* CVE-2024-43047 Qualcomm DSP Chipset メモリ読み取りの脆弱性
    * https://www.bleepingcomputer.com/news/security/qualcomm-patches-high-severity-zero-day-exploited-in-attacks/
    * https://securityonline.info/qualcomm-patched-multi-flaws-including-0-day-cve-2024-43047-rce-cve-2024-33066-cvss-9-8/
* CVE-2024-20393 Ciscoルータ、外部からの権限昇格の脆弱性
    * https://securityonline.info/privilege-escalation-and-remote-code-execution-threaten-cisco-routers-no-updates-available/ 
* CVE-2024-31449 Redis 任意のコード実行の可能性
    * https://securityonline.info/redis-patches-for-multi-flaws-including-potential-rce-cve-2024-31449/ 
* CVE-2024-9463 / CVE-2024-9464 Paloalto 未認証のコード実行の脆弱性PoCあり
    * https://www.bleepingcomputer.com/news/security/palo-alto-networks-warns-of-firewall-hijack-bugs-with-public-exploit/
    * https://securityonline.info/palo-alto-networks-issues-fix-for-critical-vulnerabilities-including-cve-2024-9463-cvss-9-9/
* CVE-2024-9680 Firefox すでに攻撃が観測されているUAFの脆弱性
    * https://www.bleepingcomputer.com/news/security/mozilla-fixes-firefox-zero-day-actively-exploited-in-attacks/
    * https://securityonline.info/firefox-zero-day-vulnerability-urgent-update-needed-to-patch-cve-2024-9680/
    * https://innovatopia.jp/cyber-security/cyber-security-news/43198/
    * https://www.darkreading.com/cyberattacks-data-breaches/critical-mozilla-firefox-zero-day-code-execution
    * https://www.theregister.com/2024/10/10/firefixed_mozilla_patches_critical_firefox/
    * https://thehackernews.com/2024/10/mozilla-warns-of-active-exploitation-in.html
* CVE-2024-9164 GitLab 未認証ユーザが任意のPipelineを実行できる脆弱性
    * https://www.bleepingcomputer.com/news/security/gitlab-warns-of-critical-arbitrary-branch-pipeline-execution-flaw/
    * https://securityonline.info/cve-2024-9164-cvss-9-6-gitlab-users-urged-to-update-now/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Oct
        * https://www.darkreading.com/vulnerabilities-threats/5-cves-microsofts-october-2024-update-patch-now
        * https://krebsonsecurity.com/2024/10/patch-tuesday-october-2024-edition/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-october-2024-patch-tuesday-fixes-5-zero-days-118-flaws/

## KEV
* CVE-2024-23113 Fortinet Multiple Products Format String Vulnerability
* CVE-2024-9379 Ivanti Cloud Services Appliance (CSA) SQL Injection Vulnerability
* CVE-2024-9380 Ivanti Cloud Services Appliance (CSA) OS Command Injection Vulnerability

# その他

* 中国グレートファイアウォール 宇宙に ～ 衛星ブロードバンドのリアルタイム検閲求める
    * https://scan.netsecurity.ne.jp/article/2024/10/08/51734.html
* ブラジル最高裁、Ｘのサービス再開許可
    * https://jp.reuters.com/business/KXEWL477GNLDTAE6O7PYQVFTPA-2024-10-08/
* 太陽フレアでNICTが注意喚起　10日深夜から数日間、通信障害などのおそれ　「宇宙システムの利用には注意が必要」
    * https://www.itmedia.co.jp/news/articles/2410/09/news193.html
    * https://www.nict.go.jp/publicity/topics/2024/10/09-2.html
* MicrosoftWord ファイルを保存するとファイルが削除される不具合。Microsoftにより修正済み
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-word-bug-that-deleted-documents-when-saving/
    * https://news.mynavi.jp/techplus/article/20241010-3042383/
* `[.]io` ドメイン終了の可能性が浮上
    * https://gigazine.net/news/20241009-domain-io/
* Windows PPTP and L2TP の非推奨化
    * https://techcommunity.microsoft.com/t5/windows-server-news-and-best/pptp-and-l2tp-deprecation-a-new-era-of-secure-connectivity/ba-p/4263956
* Windows 制限された管理者をプレビュー版に導入
    * https://www.darkreading.com/endpoint-security/windows-preview-limit-administrator-privileges
* オーストラリア、ランサムウェアへの身代金支払いを報告する法律の制定
    * https://therecord.media/australia-bill-mandatory-reporting-ransomware-payments
