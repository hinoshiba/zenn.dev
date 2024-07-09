---
title: "2024/06/30 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。早いのはGitHubです
* あくまで、発見した週に記入します
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

* UberやX, TikTok等で利用する本人 確認サービス AU10TIX データ漏洩の可能性。(AU10TIXとして、悪用確認は、無しとのこと)
    * https://news.mynavi.jp/techplus/article/20240629-2975378/
    * https://www.malwarebytes.com/blog/news/2024/06/driving-licences-and-other-official-documents-leaked-by-authentication-service-used-by-uber-tiktok-x-and-more
* オーストラリア男性、空港や飛行機でのevil twin Wifiにより起訴
    * https://thehackernews.com/2024/07/australian-man-charged-for-fake-wi-fi.html
    * https://www.darkreading.com/remote-workforce/hacker-busted-for-evil-twin-wi-fi-that-steals-airline-passenger-data
* Twilioの2要素認証アプリ Authy が、ランダムな33milionの電話番号をリークの可能性。悪用は確認できていないが、アプリの更新を推奨
    * https://www.securityweek.com/twilio-confirms-data-breach-after-hackers-leak-33m-authy-user-phone-numbers/
    * https://thehackernews.com/2024/07/twilios-authy-app-breach-exposes.html
    * https://news.mynavi.jp/techplus/article/20240705-2979511/

# 攻撃、脅威

* クボタクレジット ランサムウェア
    * https://www.itmedia.co.jp/news/articles/2407/01/news155.html
* NTT ルーマニア拠点への不正アクセスに関して
    * https://ascii.jp/elem/000/004/207/4207986/
    * https://www.security-next.com/159248
* 愛知県豊田市 委託事業者がランサムウェア被害
    * https://newsdig.tbs.co.jp/articles/-/1275326
* 京都府警が事務局の情報セキュリティー支援サイト不正アクセス
    * https://www.sankei.com/article/20240704-QLOUBGQHWNJI7BFY3LA7C5KM5U/
* 徳島県 印刷委託先事業所がランサムウェア被害
    * https://www.itmedia.co.jp/news/articles/2407/04/news126.html
* Cloudflare BGPハイジャックにより 1.1.1.1のDNSサーバへの到達が不可となっていた
    * https://www.bleepingcomputer.com/news/security/cloudflare-blames-recent-outage-on-bgp-hijacking-incident/
    * https://securityonline.info/cloudflares-1-1-1-1-dns-service-disrupted-by-bgp-hijacking-and-route-leak/

# 脆弱性
* CVE-2024-2386 WP MAPS for WordPress SQL Injectionの脆弱性
    * https://securityvulnerability.io/vulnerability/CVE-2024-2386
* CVE-2024-5535 OpenSSL 一部API関数にDoSの脆弱性。悪用は、攻撃者の制御下に限定的
    * https://www.security-next.com/159094
    * https://www.openssl.org/news/secadv/20240627.txt
* CVE-2024-6387 OpenSSH 未認証の上位権限でのRCE
    * https://securityboulevard.com/2024/07/a-playbook-for-detecting-the-openssh-vulnerability-cve-2024-6387-regresshion/
    * https://www.darkreading.com/cloud-security/regresshion-bug-threatens-takeover-of-millions-of-linux-systems
    * https://www.theregister.com/2024/07/01/regresshion_openssh/
    * https://www.bleepingcomputer.com/news/security/new-regresshion-openssh-rce-bug-gives-root-on-linux-servers/
    * https://www.securityweek.com/millions-of-openssh-servers-potentially-vulnerable-to-remote-regresshion-attack/
    * https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html
    * https://securityonline.info/cve-2024-6387-critical-openssh-unauthenticated-rce-flaw-regresshion-exposes-millions-of-linux-systems/
    * https://securityboulevard.com/2024/07/latest-openssh-vulnerability-might-impact-14m-linux-systems/
    * https://securityboulevard.com/2024/07/openssh-remote-code-execution-vulnerability-cve-2024-6387-notification/
    * https://securityboulevard.com/2024/07/regresshion-rce-vulnerability-in-openssh-server-cve-2024-6387/
    * https://news.mynavi.jp/techplus/article/20240703-2977749/
    * https://www.securityweek.com/regresshion-openssh-flaw-potential-exploitation-attempts-seen-but-mass-attacks-unlikely/
    * https://securityboulevard.com/2024/07/cve-2024-6387-new-openssh-regresshion-vulnerability-gives-hackers-root-access-on-linux-servers-700000-linux-boxes-potentially-at-risk/
* CVE-2024-38513 Fiber セッショントークンのインジェクション脆弱性
    * https://github.com/gofiber/fiber/security/advisories/GHSA-98j2-3j3p-fw2v
    * https://nvd.nist.gov/vuln/detail/CVE-2024-38513
* CVE-2024-31320 Android アプリがsetSkipPromptでプロンプトをスキップできるセキュリティ問題を修正
    * https://source.android.com/docs/security/bulletin/2024-07-01
    * https://www.securityweek.com/google-patches-25-android-flaws-including-critical-privilege-escalation-bug/
* CVE-2024-0193 1月に公開されたLinuxの権限昇格脆弱性 PoCリリース
    * https://securityonline.info/poc-exploit-published-for-linux-kernel-privilege-escalation-flaw-cve-2024-0193/
* CVE-2024-1085 2月に公開されたLinuxの権限昇格脆弱性 PoC公開
    * https://securityonline.info/linux-flaw-cve-2024-1085-poc-exploit-exposes-privilege-escalation-risk/
* CVE-2024-5261 LibreOffice データ傍受や操作を行われる可能性
    * https://securityonline.info/cve-2024-5261-cvss-10-libreoffice-patches-critical-vulnerability-in-libreofficekit/
    * https://www.security-next.com/159105
* CVE-2024-21586 Juniper SRX DoS
    * https://supportportal.juniper.net/s/article/2024-07-Out-of-Cycle-Security-Bulletin-Junos-OS-SRX-Series-Specific-valid-traffic-leads-to-a-PFE-crash-CVE-2024-21586?language=en_US
    * https://www.cisa.gov/news-events/alerts/2024/07/02/juniper-networks-releases-security-bulletin-junos-os-srx-series
    * https://securityonline.info/cve-2024-21586-juniper-srx-vulnerability-leaves-networks-open-to-attack/
* CVE-2024-36985 Splunk Enterprise RCE
    * https://www.securityweek.com/splunk-patches-high-severity-vulnerabilities-in-enterprise-product/
    * https://www.security-next.com/159257
* CVE-2024-36984 Splunk Enterprise for Windows
    * https://www.securityweek.com/splunk-patches-high-severity-vulnerabilities-in-enterprise-product/
* CVE-2024-36387 や CVE-2024-39573、CVE-2024-38476 Apache HTTPD DoSを含む不具合の脆弱性
    * https://securityonline.info/multiple-vulnerabilities-in-apache-http-server-demand-immediate-action/
    * https://www.security-next.com/159166
* CVE-2024-39884 Apache HTTPD コンテンツタイプの設定が無視され、ソースを応答してしまう可能性の脆弱性
    * https://www.security-next.com/159345
    * https://securityonline.info/apache-http-server-update-patches-critical-source-code-disclosure-flaw-cve-2024-39884/
* CVE-2024-6172 Email Subscribers by Icegram Express SQLi
    * https://jp.inoreader.com/article/3a9c6e7401f5f2bb-cve-2024-6172-critical-flaw-in-icegram-express-plugin-threatens-90000-wordpress-sites
* CVE-2024-36401 GeoServer RCE
    * https://securityonline.info/cve-2024-36401-cvss-9-8-urgent-patch-needed-for-geoserver-rce-vulnerability/
* CVE-2024-39930 Gogs 任意のコード実行等の危険性
    * https://www.sonarsource.com/blog/securing-developer-tools-unpatched-code-vulnerabilities-in-gogs-1/
    * https://securityonline.info/unpatched-gogs-vulnerabilities-a-ticking-time-bomb-for-source-code/
    * https://thehackernews.com/2024/07/critical-vulnerabilities-disclosed-in.html
* CVE-2024-39920 TCPの接続先を第三者にしられる可能性の脆弱性
    * https://vulners.com/nvd/NVD:CVE-2024-39920
    * https://nvd.nist.gov/vuln/detail/CVE-2024-39920
* CVE-2024-38366 CVE-2024-38367 CVE-2024-38368 CocoaPodsの脆弱性によりAppleデバイスサプライチェーンアタックの危機
    * https://thehackernews.com/2024/07/critical-flaws-in-cocoapods-expose-ios.html
    * https://www.darkreading.com/cloud-security/apple-cocoapods-bugs-expose-apps-code-injection
    * https://www.securityweek.com/critical-cocoapods-flaws-exposed-many-ios-macos-apps-to-supply-chain-attacks/
    * https://techcratic.com/index.php/2024/07/01/3-million-ios-and-macos-apps-were-exposed-to-potent-supply-chain-attacks/ars-technica/ars-technica/
    * https://securityboulevard.com/2024/07/cve-of-the-month-the-supply-chain-attack-hidden-for-10-years-cve-2024-38368/
    * https://news.mynavi.jp/techplus/article/20240704-2978515/
    * https://www.itmedia.co.jp/enterprise/articles/2407/04/news062.html
* CVE-2024-5943 wp-nested-pages XSS
    * https://vulners.com/nvd/NVD:CVE-2024-5943
* CVE-2024-32498 OpenStack 未認証のデータアクセスの脆弱性
    * https://securityonline.info/cve-2024-32498-critical-openstack-flaw-exposes-cloud-data-to-attackers/
* CVE-2024-37726 MSI Center 権限昇格の脆弱性。PoCあり
    * https://securityonline.info/cve-2024-37726-msi-center-flaw-exposes-windows-systems-to-privilege-escalation-attacks/
* CVE-2024-6376 MongoDB Compass システムへのコードインジェクションの脆弱性
    * https://securityonline.info/cve-2024-6376-cvss-9-8-in-mongodb-compass-exposes-systems-to-code-injection-risks/
    * https://www.security-next.com/159403
* KEV
    * CVE-2024-20399 Cisco NX-OS 管理者権限での任意のコード実行に関する脆弱性
        * https://www.bleepingcomputer.com/news/security/cisco-warns-of-nx-os-zero-day-exploited-to-deploy-custom-malware/
        * https://securityonline.info/cve-2024-20399-cisco-nx-os-zero-day-vulnerability-under-active-attack/
# その他
* Windows11 再起動ループ不具合改善版のWindowsUpdate配信開始
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-resumes-rollout-of-windows-11-kb5039302-update-for-most-users/
* Microsoft クラウドサービスに関してもCVE番号を付与していくと発表
    * https://securityonline.info/microsoft-issues-cve-numbers-for-cloud-service-vulnerabilities/
    * https://msrc.microsoft.com/blog/2024/07/toward-greater-transparency-unveiling-cloud-service-cves-ja/
* Google kvmCTFを開催
    * https://www.bleepingcomputer.com/news/security/google-now-pays-250-000-for-kvm-zero-day-vulnerabilities/
* EU攻撃者が利用していると思われる593のCobalt Strikeを停止
    * https://www.bleepingcomputer.com/news/security/europol-takes-down-593-cobalt-strike-servers-used-by-cybercriminals/
    * https://thehackernews.com/2024/07/global-police-operation-shuts-down-600.html
    * https://www.security-next.com/159268
* 「WSL2」のカーネルが「Linux 6.6 LTS」へ
    * https://forest.watch.impress.co.jp/docs/news/1605152.html
* AnyRun Windows10 64bit すべてのユーザが利用できる形に。
    * https://any.run/cybersecurity-blog/windows-10-sandbox/
* 7/15よりWindows11 開発向け仮想マシン、VMWare及びParallels版、提供一時停止
    * https://forest.watch.impress.co.jp/docs/news/1605627.html
* ChatGPTアプリケーション、会話履歴をplain textで保存。mac上に。
    * https://www.itmedia.co.jp/news/articles/2407/04/news083.html
    * https://news.mynavi.jp/techplus/article/20240704-2979220/
