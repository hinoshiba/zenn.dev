---
title: "2026/04/12 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。

# 事件事故

* Booking.comで予約データ流出、フィッシング等の注意
    * https://www.securityweek.com/booking-com-says-hackers-accessed-user-information/
    * https://www.theregister.com/2026/04/13/bookingcom_breach/

# 攻撃、脅威

* JiraSMやGitHubの通知を悪用したフィッシング攻撃、 Platform-as-a-Proxy (PaaP) model.
    * https://cybersecuritynews.com/hackers-abuse-github-and-jira-notifications/
* WindowsUpdateを狙うtyposquatting
    * https://www.malwarebytes.com/blog/scams/2026/04/this-fake-windows-support-website-delivers-password-stealing-malware

# 脆弱性

* Windows Update 4月
    * https://www.security-next.com/183438
    * https://thehackernews.com/2026/04/three-microsoft-defender-zero-days.html
    * https://thehackernews.com/2026/04/april-patch-tuesday-fixes-critical.html
    * https://gbhackers.com/windows-active-directory-flaw/
    * https://gbhackers.com/microsoft-patch-tuesday-april-2026/
    * Microsoft Defender を悪用したRedSunのPoCは公開
        * https://gbhackers.com/poc-microsoft-defender-0-day-flaw/
* CVE-2026-20204 Splunk Enterprise RCE
    * https://www.securityweek.com/splunk-enterprise-update-patches-code-execution-vulnerability/
* CVE-2026-39813 FortiSandbox 未認証のAPIアクセス
    * https://www.securityweek.com/fortinet-patches-critical-fortisandbox-vulnerabilities/
    * https://gbhackers.com/fortinet-fixes-11-security-flaws/

## KEV
* CVE-2012-1854 Microsoft Visual Basic for Applications Insecure Library Loading Vulnerability
* CVE-2020-9715 Adobe Acrobat Use-After-Free Vulnerability
* CVE-2023-21529 Microsoft Exchange Server Deserialization of Untrusted Data Vulnerability
* CVE-2023-36424 Microsoft Windows Out-of-Bounds Read Vulnerability
* CVE-2025-60710 Microsoft Windows Link Following Vulnerability
* CVE-2026-21643 Fortinet SQL Injection Vulnerability
* CVE-2026-34621 Adobe Acrobat and Reader Prototype Pollution Vulnerability
    * https://thehackernews.com/2026/04/adobe-patches-actively-exploited.html
* CVE-2026-34197 Apache ActiveMQ Improper Input Validation Vulnerability
    * https://thehackernews.com/2026/04/apache-activemq-cve-2026-34197-added-to.html

# その他
* Cloudflare、次世代エージェントを支えるエージェント型クラウドを拡張
    * https://www.cloudflare.com/ja-jp/press/press-releases/2026/cloudflare-expands-its-agent-cloud-to-power-the-next-generation-of-agents/
* OpenAI Cyberセキュリティ系モデル GPT-5.4-Cyber を追加。一部のセキュリティ関係が申請等から利用可能
    * https://x.com/openai/status/2044161906936791179
    * https://gbhackers.com/openai-extends-gpt-5-4-cyber-access/
    * https://thehackernews.com/2026/04/openai-launches-gpt-54-cyber-with.html
* WindowsServer 4月の更新後に再起動ループ
    * https://gbhackers.com/microsoft-acknowledges-reboot-loop-issue-on-windows-servers/
* Anthropic Opus 4.7 リリース
    * https://gbhackers.com/anthropic-introduces-claude-opus-4-7/
