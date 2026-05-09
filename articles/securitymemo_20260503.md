---
title: "2026/05/03 週 セキュリティニュースメモ"
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

* 台湾の特急のシステムを学生がハッキングし、逮捕
    * https://gbhackers.com/taiwan-high-speed-rail-hit-by-spoofing-attack/
    * https://www.bleepingcomputer.com/news/security/student-hacked-taiwan-high-speed-rail-to-trigger-emergency-brakes/
* マネーフォワード、GitHubリポジトリが侵害
    * https://cybersecurity-jp.com/news/113518
    * https://corp.moneyforward.com/news/info/20260501-mf-press-1/

# 攻撃、脅威
* Claude を模したマルウェア配布
    * https://gbhackers.com/fake-claude-ai-installers/
    * https://www.bleepingcomputer.com/news/security/fake-claude-ai-website-delivers-new-beagle-windows-malware/

# 脆弱性

* CVE-2026-0300 PAN-OS 管理者権限の取得
    * https://gbhackers.com/critical-palo-alto-firewall-vulnerability/
    * https://www.securityweek.com/palo-alto-networks-to-patch-zero-day-exploited-to-hack-firewalls/
    * https://gbhackers.com/cisa-issues-warning-over-palo-alto-pan-os-flaw/
    * https://thehackernews.com/2026/05/pan-os-rce-exploit-under-active-use.html
* CVE-2026-23918 Apache HTTPD DoSやRCEの可能性を持つ脆弱性
    * https://thehackernews.com/2026/05/critical-apache-http2-flaw-cve-2026.html
    * https://www.securityweek.com/critical-high-severity-vulnerabilities-patched-in-apache-mina-http-server/
    * https://gbhackers.com/apache-http-server-vulnerability-exposes-millions-rce/
    * https://www.security-next.com/184079
* Linux 権限昇格の新たな脆弱性 Dirty Frag
    * https://github.com/V4bel/dirtyfrag
    * https://thehackernews.com/2026/05/linux-kernel-dirty-frag-lpe-exploit.html
    * https://gbhackers.com/poc-exploit-for-dirty-frag-linux-kernel-vulnerability/


## KEV

* CVE-2026-6973 Ivanti Endpoint Manager Mobile (EPMM) Improper Input Validation Vulnerability 

# その他
* 米陸軍が「AIサイバー戦」演習を実施。敵のAIは凄まじい速さで、システムの脆弱性を突いてきた（海外）
    * https://news.yahoo.co.jp/articles/c84f10dc3de9e20893cab4f9447cab2c305a04fe
* シャドーAIに対抗するためのAI-BOM
    * https://www.theregister.com/security/2026/05/04/ai-boms-replace-sboms-as-way-to-track-ai-agents-and-bots/5221716
* OpenAIがアカウントへの拡張セキュリティ保護機能をリリース
    * https://www.securityweek.com/openai-rolls-out-advanced-security-for-chatgpt-accounts/
* Lets Encrypt が発行機関の潜在的な不具合により、新規証明書の発行を一時停止
    * https://cybersecuritynews.com/lets-encrypt-halts-certificate-issuance/#google_vignette
