---
title: "2025/05/17 週 セキュリティニュースメモ"
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

* Grafana GitHub Tokenが盗まれる
    * https://thehackernews.com/2026/05/grafana-github-token-breach-led-to.html
* OpenAI TanStack のサプライチェーン影響を受けたと発表
    * https://www.securityweek.com/openai-hit-by-tanstack-supply-chain-attack/
    * https://www.theregister.com/security/2026/05/15/openai-caught-in-tanstack-npm-supply-chain-chaos-after-employee-devices-compromised/5241019
    * https://securityonline.info/openai-chatgpt-codex-certificate-rotation-tanstack-incident/
* GitHub、VS Code のextenstionを悪用した攻撃により約4000の内部リポジトリの情報が流出した可能性
    * https://www.theregister.com/devops/2026/05/20/github-says-internal-repos-exfiltrated-after-poisoned-vs-code-extension-attack/5243206
    * https://www.darkreading.com/application-security/github-confirms-breach-4k-internal-repos-stolen
    * https://www.securityweek.com/github-confirms-hack-impacting-3800-internal-repositories/

# 攻撃、脅威

* node-ipc サプライチェーンアタック
    * https://gbhackers.com/popular-node-ipc-npm-library-hit-by-supply-chain-attack/

# 脆弱性

* ssh-keysign-pwn Linux /etc/shadowが見れる脆弱性
    * https://gbhackers.com/linux-ssh-keysign-pwn-flaw/
* CVE-2026-31635 DirtyDecrypt 権限昇格脆弱性 PoCリリース
    * https://thehackernews.com/2026/05/dirtydecrypt-poc-released-for-linux.html
    * https://gbhackers.com/poc-exploit-dirtydecrypt-linux-kernel-vulnerability/
* CVE-2026-42945 NGINX 任意のコード実行
    * https://gbhackers.com/critical-nginx-vulnerability/
    * https://www.securityweek.com/exploitation-of-critical-nginx-vulnerability-begins/
    * https://thehackernews.com/2026/05/nginx-cve-2026-42945-exploited-in-wild.html
    * https://www.securityweek.com/poc-code-published-for-critical-nginx-vulnerability/
* CVE-2026-8711 NGINX Javascript (njs) 任意のコード実行の可能性
    * https://www.security-next.com/184692
* CVE-2026-41702 VMWare Fusion 権限昇格の脆弱性
    * https://gbhackers.com/vmware-fusion-flaw-gain-root-privileges/

## KEV

* CVE-2026-42897 Microsoft Exchange Server Cross-Site Scripting Vulnerability

# その他
