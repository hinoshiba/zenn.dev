---
title: "2024/07/21 週 セキュリティニュースメモ"
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

* Crowdstrike Falconの世界的な不具合、修正ツールをMicrosoftが配布
    * https://techcommunity.microsoft.com/t5/intune-customer-success/new-recovery-tool-to-help-with-crowdstrike-issue-impacting/ba-p/4196959
    * https://www.securityweek.com/microsoft-says-8-5-million-windows-devices-impacted-by-crowdstrike-incident-publishes-recovery-tool/
    * https://securityboulevard.com/2024/07/new-microsoft-recovery-tool-for-crowdstrike-issue-on-windows-endpoints/
* GoogleChrome Passwordマネージャ、18時間認証情報が消える不具合。全体の2%のユーザ
    * https://www.bleepingcomputer.com/news/google/google-fixes-chrome-password-manager-bug-that-hides-credentials/
    * https://www.theregister.com/2024/07/29/google_password_manager_outage/
    * https://securityonline.info/google-patches-chrome-password-manager-bug-after-mass-outage/
    * https://news.mynavi.jp/techplus/article/20240729-2994038/

# 攻撃、脅威

* Crowdstrike FalconによるBSoDに関連する、マルウェア配布キャンペーン
    * https://thehackernews.com/2024/07/cybercriminals-exploit-crowdstrike.html
    * https://www.bleepingcomputer.com/news/security/fake-crowdstrike-fixes-target-companies-with-malware-data-wipers/
    * https://www.crowdstrike.com/blog/likely-ecrime-actor-capitalizing-on-falcon-sensor-issues/
* BreachForums v1 212,000名の情報が流出
    * https://www.bitdefender.com/blog/hotforsecurity/breachforums-data-leak-exposes-extensive-member-information/
* セキュリティ企業が誤って北朝鮮の工作員採用、ディープフェイクで潜り込む
    * https://news.mynavi.jp/techplus/article/20240725-2992619/
* 損保ジャパン出向者、千葉銀行で1万超の情報漏洩
    * https://www.nikkei.com/article/DGXZQOUB268FA0W4A720C2000000/
    * https://article.auone.jp/detail/1/3/6/16_2_r_20240727_1722041331876145
    * https://toyokeizai.net/articles/-/784835?page=2

# 脆弱性
* CVE-2024-20416 Cisco RV340などに対する任意のコード実行
    * https://securityonline.info/cisco-warns-of-unpatched-vulnerability-cve-2024-20416-in-rv340-and-rv345-routers/
* CVE-2024-36455 Symantec PAM 任意のコード実行の脆弱性
    * https://securityonline.info/broadcom-urges-immediate-patching-for-critical-symantec-pam-vulnerabilities/
    * https://www.security-next.com/160031
* CVE-2024-38437 D-Link 認証bypassの脆弱性
    * https://cvefeed.io/vuln/detail/CVE-2024-38437
* Telegram アンドロイドアプリケーション上で、悪意のあるヴィデオのより、APKファイルのインストールを促す脆弱性
    * https://securityonline.info/evilvideo-vulnerability-zero-day-threat-targets-telegram-for-android/
    * https://www.bleepingcomputer.com/news/security/telegram-zero-day-allowed-sending-malicious-android-apks-as-videos/
    * https://www.securityweek.com/telegram-zero-day-enabled-malware-delivery/
    * https://www.darkreading.com/cyberattacks-data-breaches/attackers-exploit-evilvideo-telegram-zero-day-malware
* CVE-2024-40075 Laravel XXE Injection
    * https://cvefeed.io/vuln/detail/CVE-2024-40075?utm_source=feedly
    * https://gitee.com/Q16G/laravel_bug/blob/master/laravelBug.md
    * https://securityonline.info/cve-2024-40075-xxe-vulnerability-found-in-laravel-v11-x/
* CVE-2024-33352 BlueStacks 攻撃者により任意の操作を行われる脆弱性
    * https://securityonline.info/cve-2024-33352-bluestacks-vulnerability-puts-millions-of-gamers-at-risk/
* CVE-2024-0981 Okta ブラウザプラグイン XSS
    * https://securityonline.info/okta-patches-cross-site-scripting-flaw-cve-2024-0981-in-browser-plugin/
* CVE-2024-41012 Linux kernel uaf
    * https://cvefeed.io/vuln/detail/CVE-2024-41012
* CVE-2024-1737 BIND9 キャッシュ応答が遅延する脆弱性
    * https://cvefeed.io/vuln/detail/CVE-2024-1737
    * https://www.cisa.gov/news-events/alerts/2024/07/24/isc-releases-security-advisories-bind-9
    * https://www.securityweek.com/bind-updates-resolve-high-severity-dos-vulnerabilities/
    * https://thehackernews.com/2024/07/cisa-warns-of-exploitable.html
    * https://securityonline.info/bind-security-updates-patch-your-dns-servers-now/
* CVE-2024-41110 Docker 権限昇格の可能性。Content-Length を0にすることでAuthZプラグインの認証検証に対して不正を行う脆弱性
    * https://www.bleepingcomputer.com/news/security/docker-fixes-critical-5-year-old-authentication-bypass-flaw/
    * https://securityonline.info/docker-users-beware-cve-2024-41110-cvss-10-could-lead-to-system-takeover/
    * https://jp.inoreader.com/article/3a9c6e7473aadb37-critical-docker-engine-flaw-allows-attackers-to-bypass-authorization-plugins
    * https://www.securityweek.com/docker-patches-critical-authz-plugin-bypass-vulnerability-dating-back-to-2018/
* CVE-2024-39700 JupyterLab 拡張テンプレートによる任意のコード実行
    * https://securityonline.info/cve-2024-39700-cvss-9-9-severe-flaw-in-jupyterlab-template-discovered/
* CVE-2024-3246 WordPress Plugin LiteSpeed Cache CSRF脆弱性によるXSSの可能性
    * https://securityonline.info/cve-2024-3246-litespeed-cache-plugin-vulnerability-puts-millions-of-wordpress-sites-at-risk/
* CVE-2024-6327 Progress Telerik Report Server RCEの脆弱性
    * https://docs.telerik.com/report-server/knowledge-base/deserialization-vulnerability-cve-2024-6327
    * https://www.bleepingcomputer.com/news/security/progress-warns-of-critical-rce-bug-in-telerik-report-server/
    * https://www.securityweek.com/progress-patches-critical-telerik-report-server-vulnerability/
* CVE-2024-39671 HarmonyOS セキュリティ検証不備
    * https://www.cvedetails.com/cve/CVE-2024-39671/
    * https://vuldb.com/?id.272426
* CVE-2024-37084 Spring Cloud Data Flow RCE
    * https://securityonline.info/cve-2024-37084-cvss-9-8-remote-code-execution-in-spring-cloud-data-flow/
    * https://spring.io/security/cve-2024-37084
* CVE-2024-7047 GitLab XSS
    * https://www.cvedetails.com/cve/CVE-2024-7047/
    * https://securityonline.info/gitlab-patches-six-security-flaws-urges-immediate-update/
    * https://www.security-next.com/160146
* KEV
    * CVE-2012-4792 Microsoft Internet Explorer Use-After-Free Vulnerability
    * CVE-2024-39891 Twilio Authy Information Disclosure Vulnerability

# その他

* Google 2025年8月にショートURLサービス`goo.gl`のサポートを終了。以降は、404になる予定
    * https://securityonline.info/google-url-shortener-ends-support-what-you-need-to-know-before-august-2025/
    * https://developers.googleblog.com/en/google-url-shortener-links-will-no-longer-be-available/
* Google サードパーティ製Cookieのblockを撤回
    * https://www.bleepingcomputer.com/news/security/google-rolls-back-decision-to-kill-third-party-cookies-in-chrome/
    * https://www.theregister.com/2024/07/23/google_cookies_third_party_continue/
    * https://www.securityweek.com/google-will-keep-third-party-cookies-in-chrome/
    * https://www.darkreading.com/data-privacy/google-will-not-remove-third-party-cookies-from-chrome
* Thunderbird システムトレイ通知対応
    * https://www.theregister.com/2024/07/22/mozilla_thunderbird_ffix/
* DigitalStressをテイクダウン。NCA主導
    * https://www.bleepingcomputer.com/news/security/police-infiltrates-takes-down-digitalstress-ddos-for-hire-service/
    * https://securityonline.info/operation-poweroff-major-blow-to-global-ddos-for-hire-service/
* ソフトウェア等の脆弱性関連情報に関する届出状況[2024年第2四半期（4月～6月）]
    * https://www.ipa.go.jp/security/reports/vuln/software/2024q2.html
    * https://www.security-next.com/159975
* Cloudflare WARP を攻撃のGWとして利用される例
    * https://securityonline.info/cloudflare-warp-abused-to-hijack-cloud-services-cado-security-report-reveals/
    * https://www.cadosecurity.com/news-and-events/warpscan-cloudflare-warp-abused-to-hijack-cloud-services
        * `Cado Security has observed several threads on sysadmin forums, where network operators are advised to allowlist all of Cloudflare’s IP ranges instead of just those specific to a given service, which is a serious security risk that makes their infrastructure directly vulnerable to attackers using WARP to launch their attacks.`
        * memo: 以下のURLをみつつ、WARPをアクセスしてみた感じrangeは異なりそう
            * https://www.cloudflare.com/ips/
            * memo時点、`104[.]24[.]0[.]0/14` が最も近そうではあったが、今WARPを繋ぐと、`104[.]28[.]..`だった
* 2024/07 のWindowsUpdate以降、bitlocker画面が表示されるケースがある 
    * https://www.inoreader.com/article/3a9c6e74730ba8c9-windows-july-security-updates-send-pcs-into-bitlocker-recovery
    * https://www.theregister.com/2024/07/24/windows_update_bitlocker/
* Let's Encrypt OCSP のサービスを終了。2024/07/23
    * https://letsencrypt.org/2024/07/23/replacing-ocsp-with-crls.html
    * https://securityonline.info/lets-encrypt-announces-intent-to-end-ocsp-support-a-move-towards-privacy-and-efficiency/
* Google Wizの買収、Wiz側が拒否との噂。Googleからの公式コメントは無し
    * https://www.moomoo.com/ja/news/post/41102534/cybersecurity-unicorn-wiz-inc-declines-google-s-23-billion-offer?level=1&data_ticket=1721865292764883
    * https://news.mynavi.jp/techplus/article/20240724-2991817/
* OpenAI SearchGPTをアナウンス。まだ利用はできない
    * https://www.theregister.com/2024/07/25/openai_finally_launches_searchgpt_its/
    * https://securityonline.info/openai-introduces-searchgpt-prototype/
* Windows11 バックアップが失敗する不具合を修正
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-kb5040527-update-fixes-windows-backup-failures/
* WindowsHelloに対する懸念。Micorosoftは3月に更新をリリース
    * https://securityonline.info/critical-vulnerability-in-windows-hello-for-business-discovered-by-researcher/
* Windows Server 7月アップデート、RDP不具合。ワークアラウンドあり
    * https://www.bleepingcomputer.com/news/microsoft/july-windows-server-updates-break-remote-desktop-connections/
* DNSキャッシュ汚染によるDoS攻撃、`TuDoor`
    * https://securityonline.info/tudoor-attack-new-dns-vulnerability-threatens-internet-security/
* Meta社 恐喝詐欺に関わるインスタグラムアカウント 6万3千を削除
    * https://www.bitdefender.com/blog/hotforsecurity/meta-takes-down-60-000-accounts-on-instagram-to-disrupt-nigerian-extortion-ring/
    * https://news.mynavi.jp/techplus/article/20240726-2993305/
* ニコニコ動画 8/5 サービス再開
    * https://blog.nicovideo.jp/niconews/225330.html
* 第２回フィッシングサイト撲滅チャレンジカップ 開催中
    * https://www.sankei.com/article/20240722-7K25SSJ5W5JKTBJI3WIHJNXWKU/
    * https://www.jc3.or.jp/threats/topics/article-566.html
