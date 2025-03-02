---
title: "2025/02/23 週 セキュリティニュースメモ"
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

# 脆弱性

* 昨年リリースされたParallels Desktop 権限昇格脆弱性CVE-2024-34331  PoCリリース
    * https://securityonline.info/0-day-in-parallels-desktop-allows-root-privilege-escalation-poc-released/
* CVE-2025-27364 MITRE Caldera RCEの脆弱性
    * https://securityonline.info/cve-2025-27364-cvss-10-remote-code-execution-flaw-found-in-mitre-caldera-poc-releases/
    * https://www.theregister.com/2025/02/25/10_bug_mitre_caldera/
* 1月に修正されたrsyncの脆弱性、PoCリリース CVE-2024-12084 & CVE-2024-12085
    * https://securityonline.info/cve-2024-12084-cve-2024-12085-rsync-flaws-allow-hackers-to-take-over-servers-poc-published/
* CVE-2025-20111 CISCO Nexus 3000 and 9000 DoS の脆弱性の修正
    * https://securityonline.info/cisco-warns-of-dos-vulnerability-in-nexus-3000-and-9000-series-switches-cve-2025-20111/
* CVE-2025-20029 F5 BIG-IP コマンドインジェクションの脆弱性 PoCあり
    * https://securityonline.info/cve-2025-20029-command-injection-flaw-discovered-in-f5-big-ip-system-poc-releases/
* CVE-2025-0514 LibreOffice 細工されたURLにより任意の実行の可能性
    * https://securityonline.info/cve-2025-0514-libreoffice-flaw-could-allow-unintentional-execution-of-malicious-files/
* CVE-2025-0475 GitLab XSSの脆弱性
    * https://securityonline.info/cve-2025-0475-cve-2025-0555-gitlabs-high-risk-patch-now/

## KEV
* CVE-2025-24989 Microsoft Power Pages Improper Access Control Vulnerability
* CVE-2017-3066 Adobe ColdFusion Deserialization Vulnerability
* CVE-2024-20953 Oracle Agile Product Lifecycle Management (PLM) Deserialization Vulnerability
* CVE-2024-49035 Microsoft Partner Center Improper Access Control Vulnerability
* CVE-2023-34192 Synacor Zimbra Collaboration Suite (ZCS) Cross-Site Scripting (XSS) Vulnerability

# その他
* オーストラリア政府 Kasperskyの利用を停止
    * https://www.bleepingcomputer.com/news/security/australia-bans-all-kaspersky-products-on-government-systems/
    * https://www.securityweek.com/kaspersky-banned-on-australian-government-systems/
    * https://thehackernews.com/2025/02/australia-bans-kaspersky-software-over.html
* 広告付きOfficeソフトのテスト
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-tests-ad-supported-office-apps-for-windows-users/
* マルウェア入りゲームがSteamで配信されていた
    * https://automaton-media.com/articles/newsjp/steam-malware-20250221-329184/
* Apple イギリスでのADPの提供を新規ユーザに対して終了。既存ユーザもおって。
    * https://thehackernews.com/2025/02/apple-drops-iclouds-advanced-data.html
    * https://www.bleepingcomputer.com/news/security/apple-pulls-icloud-end-to-end-encryption-feature-in-the-uk/
* Docker pullなどに制限
    * https://www.theregister.com/2025/02/22/docker_hub_pull_limits/
* Skype 5月に終了
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-confirms-its-killing-off-skype-in-may-after-14-years/
