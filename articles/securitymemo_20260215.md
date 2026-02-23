---
title: "2026/02/15 週 セキュリティニュースメモ"
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

* サイバーセキュリティインシデントに関するお知らせ / 株式会社アドバンテスト
    * https://www.advantest.com/ja/news/2026/20260219.html
        > 当社ネットワーク内の一部システムに影響を及ぼした可能性のある、ランサムウェアを伴うサイバーセキュリティインシデントが発生したことをお知らせいたします。なお、現在も本件に関する調査は継続しており、新たな事実が確認され、また、事実関係に変化が生じた場合には、本報告の内容に変更が生じることにご留意ください。
    * https://www.bleepingcomputer.com/news/security/japanese-tech-giant-advantest-hit-by-ransomware-attack/

# 攻撃、脅威

* Microsoft DNSベースのClickFix に関する情報を公開
    * https://thehackernews.com/2026/02/microsoft-discloses-dns-based-clickfix.html
    * https://thehackernews.com/2026/02/microsoft-discloses-dns-based-clickfix.html
* OpenClawのプラグインの多くにインフォスティーら系マルウェア
    * https://thehackernews.com/2026/02/researchers-find-341-malicious-clawhub.html
* ClickFix のデータ置き場所としてブラウザキャッシュを利用する例
    * https://gbhackers.com/clickfix-malware-payload/

# 脆弱性
* CVE-2026-26119 Windows Admin Center 権限昇格
    * https://gbhackers.com/critical-flaw-in-windows-admin-center-exposes/
    * https://thehackernews.com/2026/02/microsoft-patches-cve-2026-26119.html


## KEV
* CVE-2025-49113 RoundCube Webmail Deserialization of Untrusted Data Vulnerability
* CVE-2025-68461 RoundCube Webmail Cross-site Scripting Vulnerability
* CVE-2008-0015 Microsoft Windows Video ActiveX Control Remote Code Execution Vulnerability
* CVE-2020-7796 Synacor Zimbra Collaboration Suite (ZCS) Server-Side Request Forgery Vulnerability
* CVE-2024-7694 TeamT5 ThreatSonar Anti-Ransomware Unrestricted Upload of File with Dangerous Type Vulnerability
* CVE-2026-2441 Google Chromium CSS Use-After-Free Vulnerability


# その他
* AIに生成させたパスワードにパターンがあるという研究
    * https://www.malwarebytes.com/blog/news/2026/02/ai-generated-passwords-are-a-security-risk
* ChatGPT LockDownモードを追加
    * https://openai.com/index/introducing-lockdown-mode-and-elevated-risk-labels-in-chatgpt/
* Claude Code Security が早期リリースを開始
    * https://x.com/claudeai/status/2024907535145468326
    * https://www.anthropic.com/news/claude-code-security
    * https://gbhackers.com/anthropic-debuts-claude-code-security/
