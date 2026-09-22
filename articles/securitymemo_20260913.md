---
title: "2026/09/13 週 セキュリティニュースメモ"
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

* 自律型AIエージェント群、8月のHugging Face侵入の2カ月前にRubyGemsも攻撃していたと判明
    * https://www.theregister.com/security/2026/09/14/openais-malicious-bot-swarm-attacked-rubygems/5296356
* フィンテックRevolut、政府機関なりすましフィッシングでデータ侵害
    * https://www.bleepingcomputer.com/news/security/revolut-discloses-data-breach-exposing-financial-info-passports/

# 攻撃、脅威

# 脆弱性

* CVE-2026-76461 Cisco Secure Email Gatewayの重大脆弱性CVE-2026-76461、細工メール1通でroot権限奪取が実環境で悪用
    * https://www.theregister.com/security/2026/09/15/cisco-email-security-boxes-can-be-rooted-by-an-email/5296604
* CVE-2026-90894 Parallels Desktop 非管理者MacユーザーがROOT権限を奪取可能
    * https://gbhackers.com/parallels-desktop-flaw/
* Plugin4Shell Claude Code・Codex・Copilot・Gemini CLIのプラグインpin検証不備によるゼロクリックRCE
    * https://www.theregister.com/security/2026/09/17/ai-coding-agents-0-click-rce-flaw-could-hand-attackers-keys-to-the-kingdom/5297335 

## KEV

# その他
* CISA、週次脆弱性速報を廃止しリスクベースの優先度付けへ転換
    * https://www.theregister.com/security/2026/09/16/cisa-decides-weekly-vulnerability-bulletin-isnt-necessary-anymore/5296968
* ChatGPT内広告の新形式「Sponsored Agents」を試験提供開始
    * https://www.unite.ai/openai-tests-sponsored-agents-and-rolls-out-ai-tools-for-chatgpt-ads/
