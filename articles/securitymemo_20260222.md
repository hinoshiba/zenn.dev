---
title: "2026/02/22 週 セキュリティニュースメモ"
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

- 日本医科大学武蔵小杉病院 ランサムウェア被害
    - `https://www.nms.ac.jp/kosugi-h/news/_28850.html`

# 攻撃、脅威

- GitHub Codespaceに対してIssue経由で開かせることで、AIにTokenを流出させる攻撃
    https://thehackernews.com/2026/02/roguepilot-flaw-in-github-codespaces.html

# 脆弱性

- CVE-2026-25755 jsPDF Object Injection XSS
    - https://gbhackers.com/jspdf-millions-developers-exposed/
- CVE-2026-20140 Splunk DLL Hijack
    - https://advisory.splunk.com//advisories/SVD-2026-0205
- CVE-2026-22720 VMWare Aria XSS
    - https://gbhackers.com/vmware-aria-flaws/
- CVE-2025-59536 Claude Code 任意のコード実行の脆弱性
    - https://thehackernews.com/2026/02/claude-code-flaws-allow-remote-code.html
    - https://thehackernews.com/2026/02/claude-code-flaws-allow-remote-code.html
- CVE-2026-21902 Juniper RTX 未認証のコード実行
    - https://www.securityweek.com/juniper-networks-ptx-routers-affected-by-critical-vulnerability/
    - https://gbhackers.com/juniper-networks-ptx-vulnerability/


## KEV

- CVE-2026-25108 Soliton Systems K.K. FileZen OS Command Injection Vulnerability
- CVE-2022-20775 Cisco Catalyst SD-WAN Path Traversal Vulnerability
- CVE-2026-20127 Cisco Catalyst SD-WAN Controller and Manager Authentication Bypass Vulnerability 
- CVE-2025-8110 Gogs Path Traversal Vulnerability 

# その他
- Kali Linux, mcp-kali-server の公開とClaudeとの使い方
    - https://www.kali.org/blog/kali-llm-claude-desktop/
- Anthropic AI 米国国防省との利用交渉決裂。米国政府内利用禁止に。
    - https://gbhackers.com/trump-bans-anthropic-ai-in-federal-agencies/
    - https://thehackernews.com/2026/02/pentagon-designates-anthropic-supply.html
- Anthropic AI ブログを開始。退職したAIによるコメントの執筆
    - https://www.theregister.com/2026/02/26/anthropic_claude_opus_3_blog/
- Claude Code Remote を発表
    - https://gbhackers.com/claude-code-lets-users-control-terminal-sessions-remotely-from-their-phones/
