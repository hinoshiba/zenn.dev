---
title: "2026/05/25 週 セキュリティニュースメモ"
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

* 7-Eleven 18万件超えの個人情報流出
    * https://news.mynavi.jp/techplus/article/20260527-4509613/
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/7-eleven-data-breach
    * https://www.mass.gov/doc/2026-790-7-eleven-inc/download
* Carnivalクルーズ、600万人の顧客情報流出を認める
    * https://www.theregister.com/cyber-crime/2026/05/28/carnival-shinyhunters-cruised-off-with-6m-customer-records/5247808

# 攻撃、脅威

* FBI Phising as a Service, Kali365 に関して警告
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/fbi-kali365-phishing-kit-breaks-microsoft-365-accounts-no-password-required
    * https://www.ic3.gov/PSA/2026/PSA260521

# 脆弱性

* CVE‑2026‑48095 7-ZIP コード実行の可能性
    * https://gbhackers.com/multiple-7-zip-vulnerabilities-arbitrary-code-execution/
    * https://securityonline.info/7-zip-heap-buffer-overflow-cve-2026-48095/
* CVE-2026-9312 GitHub Enterprise SSRF
    * https://gbhackers.com/github-enterprise-server-3-20-3-addresses-critical-security-flaws/
    * https://www.security-next.com/185038
* CVE-2026-0257 Palo Alto PAN Unathorize access
    * https://gbhackers.com/palo-alto-pan-os-authentication-bypass/
    * https://thehackernews.com/2026/05/pan-os-globalprotect-authentication.html
    * https://securityonline.info/pan-os-authentication-bypass-flaw-exploited/
* CVE-2026-9560 macOS OpenVPN Client RCE
    * https://gbhackers.com/openvpn-connect-macos-vulnerability/
* Gogs 任意のコード実行の脆弱性
    * https://thehackernews.com/2026/05/critical-gogs-rce-vulnerability-lets.html
    * https://gbhackers.com/new-gogs-0-day-flaw/


## KEV

* CVE-2026-48172 LiteSpeed cPanel Plugin Privilege Escalation Vulnerability
* CVE-2026-8398 Daemon Tools Lite Embedded Malicious Code Vulnerability
* CVE-2026-45321 TanStack Unspecified Vulnerability
* CVE-2026-48027 Nx Console Embedded Malicious Code Vulnerability
* CVE-2026-0257 Palo Alto Networks PAN-OS Authentication Bypass Vulnerability

# その他
* Crowdstrike Glassworm botnetの停止。GoogleやShadowserver Foundationとともに。
    * https://www.theregister.com/cyber-crime/2026/05/27/crowdstrike-google-shatter-glassworm-botnet/5247337
    * https://www.crowdstrike.com/en-us/blog/inside-crowdstrike-takedown-of-a-developer-targeting-botnet/
* Anthropic ソースコードの脆弱性を検査するプラグインをリリース
    * https://gbhackers.com/anthropic-launches-free-claude-code-terminal-plugin/
* Claude Opus 4.8 リリース
    * https://gbhackers.com/claude-opus-4-8-released/
