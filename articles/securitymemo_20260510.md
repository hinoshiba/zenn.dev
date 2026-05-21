---
title: "2026/05/10 週 セキュリティニュースメモ"
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
* オンライン学習サイト Canvas がサイバー攻撃を受ける
    * https://www.securityweek.com/canvas-system-is-online-after-a-cyberattack-disrupted-thousands-of-schools/

# 攻撃、脅威
* TanStack サプライチェーン攻撃 — 84パッケージが汚染、@tanstack/react-router（週1200万DL）含む。OpenAI社員のデバイスも被害確認。
    * https://tanstack.com/blog/npm-supply-chain-compromise-postmortem

# 脆弱性
* CVE-2026-7482 Ollama メモリリークの脆弱性
    * https://thehackernews.com/2026/05/ollama-out-of-bounds-read-vulnerability.html
* Windows Update 5月
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-may
    * https://gbhackers.com/microsoft-cumulative-update-windows-11/
    * https://thehackernews.com/2026/05/microsoft-patches-138-vulnerabilities.html
    * CVE-2026-40361 Microsoft Word Zeroclick RCE
        * https://www.securityweek.com/microsoft-patches-critical-zero-click-outlook-vulnerability-threatening-enterprises/
    * CVE-2026-41096 Windows DNS Client Security Flaw Exposes Systems to Remote Code Execution
        * https://gbhackers.com/windows-dns-client-security-flaw-exposes-systems/
* BitLockerの解除できる脆弱性、PoCリリース
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/bitlocker-zero-day-poc
* CVE-2026-46300 新たなLinux権限昇格 Fragnesia
    * https://thehackernews.com/2026/05/new-fragnesia-linux-kernel-lpe-grants.html
    * https://gbhackers.com/poc-exploit-released-for-fragnesia-linux-flaw/


## KEV
* CVE-2026-20182 Cisco Catalyst SD-WAN Controller Authentication Bypass Vulnerability 


# その他
* 経産省、サイバー防護で緊急点検／電力２４社に要請
    * https://www.denkishimbun.com/archives/406634
* OpenAI 脆弱性の自動検出などのセキュリティ向け Daybreak
    * https://gbhackers.com/openai-automates-vulnerability-detection/
    * https://thehackernews.com/2026/05/openai-launches-daybreak-for-ai-powered.html
