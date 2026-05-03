---
title: "2026/04/26 週 セキュリティニュースメモ"
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

* Money Forward - 『GitHub』への不正アクセス発生に関するお知らせとお詫び（第一報）
    * https://corp.moneyforward.com/news/info/20260501-mf-press-1/
* 複数Chatworkアカウントが侵害、不正な請求書送信も - 鉄道設備機器メーカー
    * https://www.security-next.com/184004

# 攻撃、脅威
* SAP NPM パッケージサプライチェーンアタック
    * https://www.securityweek.com/sap-npm-packages-targeted-in-supply-chain-attack/
    * https://gbhackers.com/compromised-sap-npm-packages/
    * https://thehackernews.com/2026/04/sap-npm-packages-compromised-by-mini.html

# 脆弱性

* OpenClaw ポリシバイパスの脆弱性
    * https://gbhackers.com/openclaw-flaws-bypass-attacks/
* CVE-2026-3854 GitHub Git pushを利用したRCE
    * https://thehackernews.com/2026/04/researchers-discover-critical-github.html
    * https://gbhackers.com/github-com-and-enterprise-server-vulnerability/
    * https://www.securityweek.com/critical-github-vulnerability-exposed-millions-of-repositories/
* CVE-2026-42208 LiteLLM SQL Injection
    * https://securityonline.info/litellm-sql-injection-exploited-in-the-wild-cve-2026-42208/
    * https://thehackernews.com/2026/04/litellm-cve-2026-42208-sql-injection.html
* CVE-2026-31431 Linux PoE
    * https://copy.fail/
    * https://www.securityweek.com/copy-fail-logic-flaw-in-linux-kernel-enables-system-takeover/
    * https://thehackernews.com/2026/04/new-linux-copy-fail-vulnerability.html
    * https://gbhackers.com/linux-kernel-0-day-copy-fail-grants-root-access-major-distros/
    * https://securityonline.info/linux-kernel-copy-fail-root-exploit-poc-public-disclosure/
* CVE-2026-5403 WireShark Code Execution
    * https://gbhackers.com/multiple-wireshark-vulnerabilities/


## KEV
* CVE-2024-1708 ConnectWise ScreenConnect Path Traversal Vulnerability
* CVE-2026-32202 Microsoft Windows Protection Mechanism Failure Vulnerability
    * https://gbhackers.com/cisa-warns-of-windows-shell-zero-day/

# その他
* Claude Opus 4.6により本番環境含めたデータがwipeされた事件
    * https://gbhackers.com/claude-opus-4-6-powered-ai-coding-agent-wipes-production-database/
* Cloudflare AI Agentsのためのドメイン購入やdeployのインタフェースを公開
    * https://blog.cloudflare.com/agents-stripe-projects/
* MITRE ATT&CK v19 リリース
    * https://medium.com/mitre-attack/attack-v19-ff329cb65d66
* Anthropic Claude Security をEnterpriseでpublic betaリリース
    * https://gbhackers.com/claude-security-enters-public-beta/
    * https://www.securityweek.com/anthropic-unveils-claude-security-to-counter-ai-powered-exploit-surge/
