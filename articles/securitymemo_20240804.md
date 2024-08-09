---
title: "2024/08/04 週 セキュリティニュースメモ"
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

* KADOKAWA 社、ランサムウェア攻撃の情報漏洩のお知らせ、ニュースリリース
    * https://tp.kadokawa.co.jp/.assets/240805_release_f2Alq0nH.pdf
* SHARP オンラインストアサイトへの攻撃、ココロストアに加え、ヘルシオデリも。
    * https://news.goo.ne.jp/article/netkeizai/business/netkeizai-12150.html

# 脆弱性

* Linuxに対する新しいクロスキャッシュ攻撃、SLUBStick。99%の成功率で任意のメモリ読み書きが可能とのこと。詳細は、[8月のUsenx Security Symposiumで発表予定](https://www.usenix.org/conference/usenixsecurity24/presentation/maar-slubstick)
    * https://www.bleepingcomputer.com/news/security/linux-kernel-impacted-by-new-slubstick-cross-cache-attack/
    * https://securityboulevard.com/2024/08/novel-slubstick-linux-exploit-gives-attackers-full-system-control/
    * https://www.securityweek.com/new-slubstick-attack-makes-linux-kernel-vulnerabilities-more-dangerous/
    * https://thehackernews.com/2024/08/new-linux-kernel-exploit-technique.html
    * https://www.security-next.com/160619
* CVE-2024-7031 WordPress Plugin File Manager Pro 未認証のファイル編集
    * https://securityvulnerability.io/vulnerability/CVE-2024-7031
* CVE-2024-38856 Apache OFBiz 未認証のコード実行。PoCあり
    * https://seclists.org/oss-sec/2024/q3/142
    * https://www.darkreading.com/application-security/critical-apache-ofbiz-vulnerability-allows-preauth-rce
    * https://www.securityweek.com/apache-ofbiz-users-warned-of-new-and-exploited-vulnerabilities/
    * https://thehackernews.com/2024/08/new-zero-day-flaw-in-apache-ofbiz-erp.html
    * https://securityonline.info/poc-exploit-released-for-apache-ofbiz-remote-code-execution-flaw-cve-2024-38856/
* CVE-2024-42009 RoundCube XSS
    * https://www.security-next.com/160511
    * https://thehackernews.com/2024/08/roundcube-webmail-flaws-allow-hackers.html
* CVE-2024-22169: Western Digital Discovery App コード実行の脆弱性
    * https://securityonline.info/cve-2024-22169-western-digitals-wd-discovery-app-exposed-to-code-execution-vulnerability/
* CVE-2024-6472 LibreOffice マクロ署名bypassの脆弱性
    * https://www.libreoffice.org/about-us/security/advisories/CVE-2024-6472
    * https://forest.watch.impress.co.jp/docs/news/1614129.html
* CVE-2024-43044 Jenkins 外部からのライブラリ読み込みによる任意のコード実行の脆弱性
    * https://github.com/advisories/GHSA-h856-ffvv-xvr4
    * https://securityonline.info/cve-2024-43044-critical-jenkins-vulnerability-exposes-servers-to-rce-attacks/
* CVE-2024-4885 6月末に公開されたProgressの脆弱性、PoCリリース
    * https://www.cvedetails.com/cve/CVE-2024-4885/?q=CVE-2024-4885
* CVE-2024-37287 Kibana 任意のコード実行
    * https://securityonline.info/cve-2024-37287-cvss-9-9-urgent-kibana-patch-for-severe-security-vulnerability/
* CVE-2024-7532 GoogleChrome コード実行の可能性
    * https://securityonline.info/google-chrome-update-fixes-critical-code-execution-vulnerability-cve-2024-7532/
    * https://www.security-next.com/160592
* 検出できないWindowsUpdate Downgread攻撃にて、修正済みの脆弱性を悪用できる可能性を検証。BlackHat 2024にて発表
    * https://www.bleepingcomputer.com/news/microsoft/windows-update-downgrade-attack-unpatches-fully-updated-systems/
    * https://www.securityweek.com/safebreach-sounds-alarm-on-windows-update-flaws-allowing-undetectable-downgrade-attacks/
    * https://thehackernews.com/2024/08/windows-downgrade-attack-risks-exposing.html
* CVE-2024-7553 MongoDB Windows上での権限昇格
    * https://securityonline.info/mongodb-patches-high-severity-windows-vulnerability-cve-2024-7553-in-multiple-products/
* CVE-2024-42218 1Password for macOS キーチェーン上のデータを盗む脆弱性
    * https://securityonline.info/1password-updates-macos-app-to-fix-vulnerabilities-cve-2024-42218-and-cve-2024-42219/
    * https://www.theregister.com/2024/08/08/using_1password_on_mac_patch/
* CVE-2024-20451 and CVE-2024-20453 Cisco ビジネス向けのIP-Phone DoSの脆弱性。サポート切れのため適用されないデバイスもある
    * https://www.bleepingcomputer.com/news/security/cisco-warns-of-critical-rce-zero-days-in-end-of-life-ip-phones/
    * https://securityonline.info/cisco-small-business-ip-phones-affected-by-critical-vulnerabilities-no-patch/
* CVE-2024-20419 7月に修正されたCisco SSMの脆弱性、PoCリリース
    * https://securityonline.info/cisco-warns-of-public-poc-exploit-code-of-critical-cve-2024-20419-cvss-10-flaw/
* CVE-2024-42005 Django SQLi
    * https://www.security-next.com/160699
* CVE-2024-3035 GitLab LFSトークンの権限チェックにより、任意のリポジトリへアクセス可能な脆弱性
    * https://www.security-next.com/160658
* `0[.]0[.]0[.]0` にアクセスするとlocalhostへアクセスできる脆弱性
    * https://thehackernews.com/2024/08/0000-day-18-year-old-browser.html
    * https://securityonline.info/zero-day-vulnerability-18-years-of-exploiting-the-0-0-0-0-flaw/
    * https://gigazine.net/news/20240808-block-ip-address-0000/
* KEV
    * CVE-2018-0824 Microsoft COM for Windows Deserialization of Untrusted Data Vulnerability
        * https://securityonline.info/cisa-warns-of-actively-exploited-microsoft-com-for-windows-flaw/
    * CVE-2024-36971 Android Kernel Remote Code Execution Vulnerability
        * CVE-2024-36971 Google Android Kernel UAF ZeroDay
            * https://www.bleepingcomputer.com/news/security/google-fixes-android-kernel-zero-day-exploited-in-targeted-attacks/
            * https://www.securityweek.com/google-patches-android-zero-day-exploited-in-targeted-attacks/
            * https://thehackernews.com/2024/08/google-patches-new-android-kernel.html
    * CVE-2024-32113 Apache OFBiz Path Traversal Vulnerability
        * https://www.bleepingcomputer.com/news/security/cisa-warns-about-actively-exploited-apache-ofbiz-rce-flaw/

# その他

* TikTok COPPA違反で米国当局から訴訟
    * https://thehackernews.com/2024/08/doj-and-ftc-sue-tiktok-for-violating.html
    * https://www.securityweek.com/justice-department-sues-tiktok-accusing-the-company-of-illegally-collecting-childrens-data/
* 重要インフラ被害に報告義務検討
    * https://sp.m.jiji.com/article/show/3305304
* NorthAmerica及びLatinAmerica リージョンが2時間ほどダウン Azure
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-azure-outage-takes-down-services-across-north-america/
* AWS Mithra 悪意のあるドメインの予測とブロックに導入
    * https://aws.amazon.com/blogs/security/how-aws-tracks-the-clouds-biggest-security-threats-and-helps-shut-them-down/
* IPA 長期休暇における情報セキュリティ対策ページ公開
    * https://www.ipa.go.jp/security/anshin/measures/vacation.html
* CISA 最高人工知能責任者（CAIO）が就任
    * https://news.mynavi.jp/techplus/article/20240806-2997766/
* Crowdstrike センサーへのアップデートをユーザ側でコントロールできるようにする
    * https://www.darkreading.com/cyber-risk/crowdstrike-will-give-customers-control-over-falcon-sensor-content-updates
* アメリカジョージア州、自治体の公式サイトの脆弱性で誰でも勝手に「他人の有権者登録取り消しのリクエスト」を送信可能だった
    * https://gigazine.net/news/20240808-anyone-request-cancellation-voter-registrations/
* AWSにアカウント窃取の脆弱性があった
    * https://www.securityweek.com/aws-patches-vulnerabilities-potentially-allowing-account-takeovers/
