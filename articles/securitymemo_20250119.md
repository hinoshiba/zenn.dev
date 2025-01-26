---
title: "2025/01/19 週 セキュリティニュースメモ"
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

* アトラシアン、Bitbucket Cloud に障害
    * https://www.theregister.com/2025/01/21/atlassian_bitbucket_cloud_outage/atlassian_bitbucket_cloud_outage
    * https://www.bleepingcomputer.com/news/technology/bitbucket-services-hard-down-due-to-major-worldwide-outage/
* 快活CLUB サイバー攻撃で会員情報一部漏えいの可能性
    * https://www3.nhk.or.jp/news/html/20250121/k10014699481000.html
    * https://www.nikkei.com/article/DGXZQOUC21AN60R20C25A1000000/
    * https://www.security-next.com/166372

# 攻撃、脅威
* Google広告に表示されるhomebrewのリンク偽ページ誘導。curlで異なる配布元から悪意のあるbrewをインストール
    * https://x.com/ryanchenkie/status/1880730173634699393
    * https://www.bleepingcomputer.com/news/security/fake-homebrew-google-ads-target-mac-users-with-malware/
    * https://securityonline.info/homebrew-phishing-site-appears-in-google-search-raising-concerns/
* Cloudflare 5.6TbpsのDDoS攻撃を軽減
    * https://www.bleepingcomputer.com/news/security/cloudflare-mitigated-a-record-breaking-56-tbps-ddos-attack/

# 脆弱性

* CVE-2024-54887 TP-Link 任意のコード実行の脆弱性
    * https://securityonline.info/tp-link-vulnerability-poc-exploit-for-cve-2024-54887-reveals-remote-code-execution-risks/
* CVE-2025-0411 7-Zip 展開時にMotWをファイルへ伝搬しない脆弱性
    * https://securityonline.info/cve-2025-0411-7-zip-security-vulnerability-enables-code-execution-update-now/
    * https://www.bleepingcomputer.com/news/security/7-zip-fixes-bug-that-bypasses-the-windows-motw-security-mechanism-patch-now/
* CVE-2024-49138 12月に修正されたWindows 権限昇格の脆弱性、PoCリリース
    * https://securityonline.info/zero-day-vulnerability-in-windows-exploited-cve-2024-49138-poc-code-released/
* CVE-2025-21535 Oracle WebLogic DoS
    * https://securityboulevard.com/2025/01/oracle-weblogic-server-remote-code-execution-and-denial-of-service-vulnerability-cve-2025-21535-cve-2025-21549/
    * https://securityonline.info/cve-2025-21535-cvss-9-8-vulnerability-in-oracle-weblogic-server-could-lead-to-remote-code-execution/
* CVE-2025-0314 GitLab XSS
    * https://securityonline.info/cve-2025-0314-gitlab-releases-patch-for-xss-exploit/
* CVE-2025-20156 Cisco Meeting Management Software 権限昇格の脆弱性
    * https://securityonline.info/cve-2025-20156-cvss-9-9-cisco-meeting-management-flaw-allows-for-privilege-escalation/
* CVE-2025-20128 ClamAV DoSの脆弱性。PoCあり
    * https://securityonline.info/proof-of-concept-found-for-clamav-dos-flaw-cve-2025-20128/
* 2024/10月に修正されたMicrosoft Configuration ManagerのPoCリリース CVE-2024-43468
    * https://securityonline.info/cve-2024-43468-cvss-9-8-microsoft-configuration-manager-exploit-revealed-with-poc-code/

## KEV
* CVE-2020-11023 JQuery Cross-Site Scripting (XSS) Vulnerability
* CVE-2025-23006 SonicWall SMA1000 Appliances Deserialization Vulnerability

# その他
* TikTok アメリカでのサービス停止 1/19
    * https://www.bleepingcomputer.com/news/software/tiktok-shuts-down-in-the-us-as-trump-throws-the-company-a-lifeline/
    * https://thehackernews.com/2025/01/tiktok-goes-dark-in-us-as-federal-ban.html
* Outlookがクラッシュする不具合へのワークアラウンド
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-shares-temp-fix-for-outlook-crashing-when-writing-emails/
* CVEProject がパワーアップ。CISAのVulnrichmentが含まれるようになる
    * https://www.cisa.gov/news-events/news/unlocking-vulnrichment-enriching-cve-data
* LinkedIn プライベートDMをAIの学習に用い、非難
    * https://www.theregister.com/2025/01/22/linkedin_sued_for_allegedly_training/
* JVN iPedia と MyJVN サービスがシステムメンテナンス、1 / 31 ～ 2 / 3
    * https://scan.netsecurity.ne.jp/article/2025/01/23/52209.html
* WSUSによるドライバの同期が4/18に終了することをアナウンス
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-deprecate-wsus-driver-synchronization-in-90-days/
