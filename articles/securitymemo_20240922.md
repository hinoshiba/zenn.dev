---
title: "2024/09/22 週 セキュリティニュースメモ"
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

* Doctor Webに標的型攻撃 - マルウェアDB配信を一時停止
    * https://www.security-next.com/162131
* 信州大で学生ら約4100人分の情報が漏洩か　外部から不正アクセス
    * https://www.asahi.com/articles/ASS9W34LWS9WUOOB002M.html

# 脆弱性

* CVE-2024-4278 GitLab パスワードが漏洩する脆弱性
    * https://www.security-next.com/162222
* CVE-2024-38286 Apache Tomcat DoSの脆弱性。6月の更新で修正済み
    * https://www.security-next.com/162165
* CVE-2024-47045 e-Tax インストーラの権限昇格の脆弱性
    * https://www.security-next.com/162168
* CVE-2024-0132 NVIDIA Container toolkit コンテナエスケープによるホストコンピュータへの侵害の可能性
    * https://www.theregister.com/2024/09/26/critical_nvidia_bug_container_escape/
    * https://thehackernews.com/2024/09/critical-nvidia-container-toolkit.html
    * https://securityonline.info/cve-2024-0132-cvss-9-0-critical-vulnerabilities-found-in-nvidia-container-toolkit/
* CVE-2024-47076, CVE-2024-47175, CVE-2024-47176, CVE-2024-47177 UNIX Printing System (CUPS) の脆弱性によるRCE
    * https://x.com/HunterMapping/status/1839506035834282464
    * https://www.security-next.com/162302
    * https://securityboulevard.com/2024/09/cve-2024-47076-cve-2024-47175-cve-2024-47176-cve-2024-47177-frequently-asked-questions-about-common-unix-printing-system-cups-vulnerabilities/
    * https://www.bleepingcomputer.com/news/security/cups-flaws-enable-linux-remote-code-execution-but-theres-a-catch/
    * https://securityonline.info/critical-cups-vulnerabilities-expose-linux-and-other-systems-to-remote-attacks/
    * https://securityboulevard.com/2024/09/remote-code-execution-vulnerability-alert-of-unix-cups-print-service-cve-2024-47076-cve-2024-47175-cve-2024-47177/
* CVE-2024-46461 VLC Media Player任意のコード実行
    * https://securityonline.info/vlc-media-player-update-needed-cve-2024-46461-discovered/
* CVE-2024-8275 WordPress Plugin The Event Calender SQLi
    * https://securityonline.info/critical-sql-injection-vulnerability-discovered-in-the-events-calendar-wordpress-plugin-cve-2024-8275/
* CVE-2024-7479 and CVE-2024-7481 TeamViewr 権限昇格の脆弱性
    * https://securityonline.info/teamviewer-urges-users-to-patch-privilege-escalation-flaws-cve-2024-7479-and-cve-2024-7481/
* CVE-2024-9014 pgAdmin 未認証のアクセス
    * https://securityonline.info/cve-2024-9014-cvss-9-9-pgadmins-critical-vulnerability-puts-user-data-at-risk/
## KEV
* CVE-2024-7593 Ivanti Virtual Traffic Manager Authentication Bypass Vulnerability
    * https://securityonline.info/cisa-warns-of-actively-exploited-ivanti-vtm-flaw-cve-2024-7593-cvss-9-8-poc-published/
# その他

* Telegram 利用規約を更新。法的リクエストの場合、IPアドレスや電話番号を捜査当局に渡すことがある
    * https://www.theregister.com/2024/09/23/telegram_tcs_suspect_info/
    * https://www.bleepingcomputer.com/news/security/telegram-now-shares-users-ip-and-phone-number-on-legal-requests/
    * https://www.bitdefender.com/blog/hotforsecurity/telegrams-new-privacy-policy-law-enforcement-request-now-cover-a-much-broader-base/
* Kaspersky UltraAVを自動deploy
    * https://www.darkreading.com/application-security/kaspersky-rolls-back-us-customers-ultraav
* 「WordPress.org」がホスティングサービス「WP Engine」からのアクセスを遮断
    * https://www.security-next.com/162233
    * https://www.bleepingcomputer.com/news/security/automattic-blocks-wp-engines-access-to-wordpress-resources/
    * https://www.theregister.com/2024/09/26/wordpressorg_denies_service_to_wp/
* Recall は、オプトインかつ、特定アプリのみ無効化できる様子
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-recall-now-can-be-removed-is-more-secure/
