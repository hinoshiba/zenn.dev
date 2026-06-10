---
title: "2026/06/07 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。

# 事件事故

# 攻撃、脅威

* ネットワークQoSを操作しEDRの検知の通信を妨害するテクニック、EDRChoker
    * https://gbhackers.com/edrchoker-tool-abuses-windows-qos-policies/

# 脆弱性

* CVE-2026-50751 Checkpoint VPN 認証bypass
    * https://gbhackers.com/check-point-vpn-zero-day/
    * https://www.securityweek.com/check-point-vpn-zero-day-exploited-in-qilin-ransomware-attacks/
* Windows Update 6月
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-jun
    * https://cybersecuritynews.com/microsoft-patch-tuesday-june-2026/


## KEV

* CVE-2026-42271 BerriAI LiteLLM Command Injection Vulnerability
* CVE-2026-50751 Check Point Security Gateway Improper Authentication Vulnerability
* CVE-2026-7473 Arista Extensible Operating System Incomplete Comparison with Missing Factors Vulnerability
* CVE-2026-11645 Google Chromium V8 Out-of-Bounds Read and Write Vulnerability
* CVE-2026-20245 Cisco Catalyst SD-WAN Manager Improper Encoding or Escaping of Output Vulnerability

# その他
* Apple 侵害されたパスワードの自動変更機能を発表
    * https://www.bleepingcomputer.com/news/apple/new-apple-feature-automatically-changes-your-compromised-passwords/
* ChatGPT LockDown Modeをリリース
    * https://www.securityweek.com/openai-rolling-out-chatgpt-account-security-controls/
    * https://securityonline.info/chatgpt-lockdown-mode/
* 利用しているプロジェクトの脆弱性を確認するCVE Lite CLI
    * https://jp.inoreader.com/article/3a9c6e763effaf39-owasp-incubator-project-helps-developers-find-and-fix-vulnerable-dependencies-in-seconds
* Anthropic Claude Fable 5 を公開。Mythosクラスと表記。
    * https://www.securityweek.com/anthropic-launches-claude-fable-5-mythos-class-ai-with-cybersecurity-guardrails/
* Microsoft Defender for Endpointにて、インバウンドRPCの監視機能が追加
    * https://gbhackers.com/microsoft-defender-adds-monitoring-for-rpc-protocol/
