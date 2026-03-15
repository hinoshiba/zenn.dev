---
title: "2026/03/08 週 セキュリティニュースメモ"
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

# 攻撃、脅威
* CloudflareのCaptiveを突破するスクリプトについて
    * https://x.com/ihtesham2005/status/2030586222868136096?s=12
* Claude CodeのInstallFix
    * https://www.darkreading.com/cloud-security/installfix-attacks-fake-claude-code
    * https://pushsecurity.com/blog/installfix/
* 2025年からおきているnpmパッケージのキャンペーン、PhantomRavenに関する記事
    * https://gbhackers.com/phantomraven-malware/

# 脆弱性

* CVE-2026-27577 n8n sandbox escape rce
    * https://thehackernews.com/2026/03/critical-n8n-flaws-allow-remote-code.html
*  CVE-2025-54820 FortiManager 遠隔からのコード実行
    * https://gbhackers.com/fortinet-fortimanager-fgtupdates-flaw/
* Windows Update 3月
    * https://www.darkreading.com/application-security/microsoft-patches-83-cves-march-update
    * https://krebsonsecurity.com/2026/03/microsoft-patch-tuesday-march-2026-edition/
    * CVE-2026-26110 Office コード実行　
        * https://gbhackers.com/critical-vulnerability-in-microsoft-office/
    * CVE-2026-26127 DoS
        * https://gbhackers.com/microsoft-net-0-day-flaw-denial-of-service-attacks/
    * CVE-2026-21262 MSSQL 権限昇格の可能性
        * https://gbhackers.com/microsoft-sql-server-zero-day-exposes-privilege-escalation-risk-for-users/


## KEV
* CVE-2021-22054 Omnissa Workspace ONE Server-Side Request Forgery
* CVE-2025-26399 SolarWinds Web Help Desk Deserialization of Untrusted Data Vulnerability
* CVE-2026-1603 Ivanti Endpoint Manager (EPM) Authentication Bypass Vulnerability
* CVE-2025-68613 n8n Improper Control of Dynamically-Managed Code Resources Vulnerability
* CVE-2026-3909 Google Skia Out-of-Bounds Write Vulnerability
* CVE-2026-3910 Google Chromium V8 Unspecified Vulnerability

# その他
* フィッシング対策ツールtop10
    * https://gbhackers.com/best-anti-phishing-tools/
* Microsoft 365 E7 発表。AIの利用
    * https://microsoftpartners.microsoft.com/abs/Blog/?title=Introducing%20Microsoft%20365%20E7:%20The%20Frontier%20Suite
* Kali Linux上にローカルLLMを構築するデモブログ
    * https://www.kali.org/blog/kali-llm-ollama-5ire/
* INTERPOL 45,000の悪意のあるIPアドレスをtake down
    * https://www.interpol.int/en/News-and-Events/News/2026/45-000-malicious-IP-addresses-taken-down-in-international-cyber-operation
    * https://thehackernews.com/2026/03/interpol-dismantles-45000-malicious-ips.html
* Apple Corunaに対するパッチを古いデバイスに配信
    * https://www.securityweek.com/apple-updates-older-ios-versions-to-patch-coruna-exploits/
    * https://gbhackers.com/apple-releases-emergency-ios-15-8-7-update/
    * https://thehackernews.com/2026/03/apple-issues-security-updates-for-older.html
