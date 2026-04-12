---
title: "2026/04/05 週 セキュリティニュースメモ"
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

* 名古屋市が廃止したドメイン名を第三者が再取得、注意を呼びかけ
    * https://scan.netsecurity.ne.jp/article/2026/04/06/54982.html

# 攻撃、脅威
* GPUBreach gpuベースの権限昇格テクニック
    * https://www.securityweek.com/gpubreach-root-shell-access-achieved-via-gpu-rowhammer-attack/
    * https://thehackernews.com/2026/04/new-gpubreach-attack-enables-full-cpu.html
* WindowsDefender 権限昇格の可能性。ゼロデイ
    * https://gbhackers.com/windows-defender-0-day-published-online/
* macOS Clickfix scripteditorを利用した版
    * https://www.bleepingcomputer.com/news/security/new-macos-stealer-campaign-uses-script-editor-in-clickfix-attack/
* 「CPU-Z」「HWMonitor」にマルウェアが混入か
    * https://forest.watch.impress.co.jp/docs/news/2100780.html
    * https://www.reddit.com/r/pcmasterrace/comments/1sh4e5l/warning_hwmonitor_163_download_on_the_official/
    * https://dailydarkweb.net/cpuid-website-compromised-cpu-z-and-hwmonitor-serve-malware/
* OpenAI mac関係のアプリに対して、サプライチェーン攻撃の影響。影響のないバージョンへの更新をユーザへ呼びかけ
    * https://x.com/OpenAI/status/2042780052669239782?s=20

# 脆弱性

* CVE-2026-34040 Docker認証bypass
    * https://thehackernews.com/2026/04/docker-cve-2026-34040-lets-attackers.html
* CVE-2026-33784 Junos 遠隔からのコード実行の脆弱性
    * https://www.securityweek.com/juniper-networks-patches-dozens-of-junos-os-vulnerabilities/
* CVE-2026-5173 GitLab 認証bypassの脆弱性
    * https://gbhackers.com/gitlab-addresses-multiple-vulnerabilities/
* CVE-2026-34621 Adobe Acrobat Reader プロトタイプ汚染
    * https://www.security-next.com/183306


## KEV
* CVE-2026-35616 - Fortinet FortiClient EMS Improper Access Control Vulnerability
    * https://www.securityweek.com/fortinet-rushes-emergency-fixes-for-exploited-zero-day/
* CVE-2026-1340 Ivanti Endpoint Manager Mobile (EPMM) Code Injection Vulnerability

# その他
* 流通ISAC 発足
    * https://prtimes.jp/main/html/rd/p/000000268.000060129.html
* Microsoft AIエージェントのセキュリティツールキット公開
    * https://socket.dev/blog/microsoft-open-source-toolkit-for-ai-agent-runtime-security
* Anthropic OpenClawへのサブスクリプション利用を停止
    * https://www.theregister.com/2026/04/06/anthropic_closes_door_on_subscription/
* Claude Codeのセキュリティルールが50件を超えると読み込まないバグがあった
    * https://gbhackers.com/critical-claude-code-flaw/
* Claude Mythos Preview 高性能すぎるため、一部企業に限定して提供
* MITRE 金融詐欺防御フレームワークをリリース
    * https://ctid.mitre.org/projects/fight-financial-fraud/
* EmoCheck 配布終了のお知らせ
    * https://www.jpcert.or.jp/press/2026/PR20260410.html
