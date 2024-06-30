---
title: "2024/06/23 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
* あくまで、発見した週に記入します
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威
* CDK Globalsにサイバー攻撃によりサービス停止
    * https://www.darkreading.com/cloud-security/cdk-attack-contingency-planning-critical-saas-customers
    * https://www.bleepingcomputer.com/news/security/cdk-warns-threat-actors-are-calling-customers-posing-as-support/
* JAXAの不正アクセスの件が公表
    * https://cybersecurity-jp.com/news/98098
* LAの統一学区（The Los Angeles Unified School District）に関係するSnowFake上から盗まれたデータ。 hacker forumで発売される
    * https://www.bleepingcomputer.com/news/security/los-angeles-unified-confirms-student-data-stolen-in-snowflake-account-hack/
* ANYRUN フィッシング被害により電子メールが確認を受ける。本番環境への影響はないとのこと
    * https://securityonline.info/any-run-confirms-security-incident-involving-employee-email-compromise/
    * https://x.com/anyrun_app/status/1804157392935870466
    * https://www.securityweek.com/malware-sandbox-any-run-targeted-in-phishing-attack/
* WordPress Plugin のいくつかに悪意のあるバックドアが含まれる
    * https://www.bleepingcomputer.com/news/security/plugins-on-wordpressorg-backdoored-in-supply-chain-attack/
    * https://www.darkreading.com/cloud-security/wordpress-supply-chain-attack-multiple-plug-ins
    * https://thehackernews.com/2024/06/multiple-wordpress-plugins-compromised.html
    * https://www.security-next.com/158850
    * https://securityboulevard.com/2024/06/wordpress-plugin-malware-richixbw/
    * https://news.mynavi.jp/techplus/article/20240628-2973724/
* Polyfill.io が売却される。マルウェアが混入され多くのサイトへ影響の可能性
    * https://news.livedoor.com/article/detail/26673687/
    * https://www.bleepingcomputer.com/news/security/cloudflare-we-never-authorized-polyfillio-to-use-our-name/
    * https://www.securityweek.com/polyfill-domain-shut-down-as-owner-disputes-accusations-of-malicious-activity/
    * https://news.mynavi.jp/techplus/article/20240628-2974852/
* APT29 がTeamViewerのネットワークへ侵入。顧客データが影響を受けた証拠は特にないとのこと
    * https://www.darkreading.com/cyberattacks-data-breaches/teamviewer-network-segmentation-apt29-attack
    * https://www.theregister.com/2024/06/28/teamviewer_russia/
    * https://www.bleepingcomputer.com/news/security/teamviewer-links-corporate-cyberattack-to-russian-state-hackers/
    * https://thehackernews.com/2024/06/teamviewer-detects-security-breach-in.html
    * https://www.theregister.com/2024/06/28/teamviewer_network_breach/

# 脆弱性

* CVE-2024-5739 LINE UXSS
    * https://www.security-next.com/158827
    * https://news.mynavi.jp/techplus/article/20240624-2971510/
* CVE-2024-5756: WordPress Plugin Email Subscribers SQLi
    * https://securityonline.info/cve-2024-5756-cvss-9-8-critical-icegram-express-flaw-puts-90000-wordpress-sites-at-risk/
* CVE-2024-27815: Apple 6月中旬に修正したカーネル上で任意のコードを実行できる脆弱性、PoCリリース
    * https://www.inoreader.com/article/3a9c6e740fcc85d5-cve-2024-27815-apple-xnu-kernel-vulnerability-uncovered-poc-code-released
* CVE-2024-37032: ローカルでのLLM実行OSS Ollama 任意のコード実行の脆弱性
    * https://thehackernews.com/2024/06/critical-rce-vulnerability-discovered.html
* CVE-2024-37231: WordPress Plugin Salon booking system。Pathトラバーサルの脆弱性
    * https://patchstack.com/database/vulnerability/salon-booking-system/wordpress-salon-booking-system-plugin-9-9-arbitrary-file-deletion-vulnerability
* CVE-2024-0762: Lenvo端末においてUEFI上の不具合から、バッファオーバフローの脆弱性の可能性
    * https://www.security-next.com/158794
    * https://news.mynavi.jp/techplus/article/20240624-2970871/
* CVE-2024-0087: 5月に公表されたNVIDIA Tritonの脆弱性。PoCリリース
    * https://securityonline.info/poc-published-for-critical-nvidia-triton-inference-server-vulnerabilities/
* CVE-2024-2003: ESET Windows上で権限昇格の脆弱性
    * https://securityonline.info/eset-issues-security-patch-for-privilege-escalation-flaw-in-windows-products/
* CVE-2024-5806 MOVEit Transfer 未認証のユーザによるファイルアップロード
    * https://www.darkreading.com/remote-workforce/fresh-moveit-bug-under-attack-disclosure
    * https://www.bleepingcomputer.com/news/security/hackers-target-new-moveit-transfer-critical-auth-bypass-bug/
    * https://thehackernews.com/2024/06/new-moveit-transfer-vulnerability-under.html
    * https://www.securityweek.com/exploitation-attempts-target-new-moveit-transfer-vulnerability/
    * https://www.security-next.com/158957
* CVE-2024-6290 to CVE-2024-6293 Google Chrome uafの脆弱性
    * https://www.securityweek.com/chrome-126-update-patches-memory-safety-bugs/
* CVE-2023-24871 昨年3月に修正されたWindows Bluetoothに関する脆弱性。PoCリリース
    * https://securityonline.info/researcher-unveils-poc-for-windows-bluetooth-service-rce-vulnerability/
* CVE-2024-5746 GHE ユーザ権限で管理者任意のコード実行の脆弱性
    * https://www.security-next.com/158843
* WP 6.5.5 リリース。XSS修正他
    * https://www.security-next.com/158839
* CVE-2024-27867 AirPods等に盗聴の脆弱性
    * https://www.darkreading.com/vulnerabilities-threats/apple-airpods-bug-allows-eavesdropping
    * https://thehackernews.com/2024/06/apple-patches-airpods-bluetooth.html
    * https://www.security-next.com/158955
    * https://news.mynavi.jp/techplus/article/20240627-2974525/
* CVE-2024-5655 GitLab パイプライン実行のユーザ偽装
    * https://about.gitlab.com/releases/2024/06/26/patch-release-gitlab-17-1-1-released/
    * https://www.bleepingcomputer.com/news/security/critical-gitlab-bug-lets-attackers-run-pipelines-as-any-user/
    * https://securityonline.info/cve-2024-5655-gitlab-vulnerability/
    * https://www.darkreading.com/application-security/critical-gitlab-bug-threatens-software-development-pipelines
    * https://thehackernews.com/2024/06/gitlab-releases-patch-for-critical-cicd.html
* CVE-2024-37085 ESXi 認証バイパスの脆弱性。ADを利用している場合に影響がある
    * https://support.broadcom.com/web/ecx/support-content-notification/-/external/content/SecurityAdvisories/0/24505
    * https://www.security-next.com/158909
* CVE-2024-5756 WordPress Plugin Icegram Express SQLi
    * https://www.security-next.com/158904
* CVE-2024-5276 Fotra File Cytalist RCEの脆弱性。PoCあり
    * https://securityonline.info/cve-2024-5276-cvss-9-8-critical-sqli-flaw-in-fortra-filecatalyst-workflow-poc-available/
    * https://thehackernews.com/2024/06/critical-sqli-vulnerability-found-in.html
    * https://www.securityweek.com/fortra-patches-critical-sql-injection-in-filecatalyst-workflow/
* CVE-2024-36072 CoCoSys社のDLP製品に対するRCE
    * https://securityonline.info/cve-2024-36072-unauthenticated-rce-flaw-in-cososys-endpoint-protector
* CVE-2024-2973 Juniper Session  Smart Router 認証bypassの脆弱性
    * https://thehackernews.com/2024/06/teamviewer-detects-security-breach-in.html
    * https://www.security-next.com/159040
    * https://www.bleepingcomputer.com/news/security/juniper-releases-out-of-cycle-fix-for-max-severity-auth-bypass-flaw/
* KEV追加
    * CVE-2020-13965 Roundcube XSS

# その他
* MMCを利用したGrimResourceと呼ばれる新たなる攻撃手法
    * https://www.bleepingcomputer.com/news/security/new-grimresource-attack-uses-msc-files-and-windows-xss-flaw-to-breach-networks/
    * https://thehackernews.com/2024/06/new-attack-technique-exploits-microsoft.html
    * https://news.mynavi.jp/techplus/article/20240627-2972990/
* シスコ、東京にサイバーセキュリティCoEを開設
    * https://news.mynavi.jp/techplus/article/20240621-2970215/
* Kasperskey製品、米国の当局で禁止措置。他
    * https://thehackernews.com/2024/06/us-bans-kaspersky-software-citing.html
    * https://www.securityweek.com/us-bans-kaspersky-software/
    * https://securityboulevard.com/2024/06/u-s-bans-sale-of-kaspersky-cybersecurity-software/
    * https://thehackernews.com/2024/06/us-treasury-sanctions-12-kaspersky.html
    * https://news.mynavi.jp/techplus/article/20240626-2970870/
* GoogleChrome Core のEnterprise機能、ポリシー配布が追加
    * https://www.securityweek.com/google-unveils-new-chrome-enterprise-core-features-for-it-security-teams/
    * https://www.theregister.com/2024/06/26/google_chrome_enterprise/
* Windows11 06/26リリースの更新プログラム適用後に一部端末が起動しなくなる不具合発生中
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-pulls-june-windows-11-kb5039302-update-causing-repeated-restarts/
* BlackSuitランサムウェア集団がKADOKAWAを攻撃したとの公開
    * https://www.bleepingcomputer.com/news/security/blacksuit-ransomware-gang-claims-attack-on-kadokawa-corporation/
    * https://www.ransomlook.io/group/black%20suit
