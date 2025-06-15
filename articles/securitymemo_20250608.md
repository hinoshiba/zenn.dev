---
title: "2025/06/08 週 セキュリティニュースメモ"
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

* 損保ジャパン、約1750万件の顧客情報流出の可能性　不正アクセスで
    * https://www.newsweekjapan.jp/headlines/business/2025/06/555715.php
* ソフトバンク　契約者の氏名や住所など約14万件の個人情報漏えいか
    * https://newsdig.tbs.co.jp/articles/withbloomberg/1972637?display=1
    * https://news.yahoo.co.jp/articles/c707c32acb198d191565d38a4823f5dd7597e2a8
* Cloudflare Google Cloudの障害影響でサービス一時停止
    * https://www.bleepingcomputer.com/news/technology/google-cloud-and-cloudflare-hit-by-widespread-service-outages/
    * https://www.bleepingcomputer.com/news/security/cloudflare-outage-not-caused-by-security-incident-data-is-safe/
    * Googleクラウドの特定機能サービスダウンについて
        * https://www.bleepingcomputer.com/news/google/google-links-massive-cloud-outage-to-api-management-issue/


# 攻撃、脅威

* INTERPOL、69種類のマルウェアに関連する20,000以上の悪質なIPアドレスを駆除した
    * https://thehackernews.com/2025/06/interpol-dismantles-20000-malicious-ips.html


# 脆弱性

* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-jun
        * https://www.theregister.com/2025/06/11/microsoft_slows_windows_11_24h2/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-june-2025-patch-tuesday-fixes-exploited-zero-day-66-flaws/
    * CVE
        * CVE-2025-33073 SMB権限昇格、PoCあり
            * https://securityonline.info/windows-smb-flaw-cve-2025-33073-system-privilege-escalation-via-kerberos-poc-available/
* CVE-2025-32711 Microsoft 365 EchoLeak
    * https://www.darkreading.com/application-security/researchers-detail-zero-click-copilot-exploit-echoleak
    * https://www.securityweek.com/echoleak-ai-attack-enabled-theft-of-sensitive-data-via-microsoft-365-copilot/
    * https://news.mynavi.jp/techplus/article/20250612-3351994/
* CVE-2025-4278 GitLab HTMLインジェクションによりアカウント奪取の脆弱性
    * https://www.bleepingcomputer.com/news/security/gitlab-patches-high-severity-account-takeover-missing-auth-issues/
    * https://securityonline.info/urgent-gitlab-security-alert-high-severity-flaws-allow-account-takeover-code-injection/
* CVE-2025-2884 TPM 2.0 データが読み取られる可能性
    * https://securityonline.info/tpm-2-0-flaw-cve-2025-2884-exposes-sensitive-data-disrupts-trusted-computing/


## KEV
* CVE-2025-24016 Wazuh Server Deserialization of Untrusted Data Vulnerability
* CVE-2025-33053 Web Distributed Authoring and Versioning (WebDAV) External Control of File Name or Path Vulnerability
* CVE-2025-32433 Erlang Erlang/OTP SSH Server Missing Authentication for Critical Function Vulnerability 
* CVE-2024-42009 RoundCube Webmail Cross-Site Scripting Vulnerability 


# その他
* iOS 26から、iOSパスワードマネージャにて、履歴等の機能がサポートされる
    * https://securityonline.info/ios-26-password-app-gains-major-upgrade-view-full-history-of-saved-credentials/
