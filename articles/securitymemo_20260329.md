---
title: "2026/03/29 週 セキュリティニュースメモ"
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

* マイナビ 不正アクセス: クラウドが不正アクセス受け個人情報流出　マイナビ、ユーザー情報7万件など
    * https://www.mynavi.jp/json-topic/52681/
    * https://x.com/H4ckmanac/status/2039611983373238323?s=20
    * https://www.itmedia.co.jp/news/articles/2604/02/news075.html
* Claude Code npmのmapによりソースコード流出
    * https://www.bleepingcomputer.com/news/artificial-intelligence/claude-code-source-code-accidentally-leaked-in-npm-package/
    * 配布していたリポジトリは、DMCA takedown
        * https://github.com/github/dmca/blob/master/2026/03/2026-03-31-anthropic.md
    * 偽物やマルウェア入り版が配布
        * https://www.bitdefender.com/en-us/blog/hotforsecurity/claude-code-leak-github-vidar-malware
        * https://www.bleepingcomputer.com/news/security/claude-code-leak-used-to-push-infostealer-malware-on-github/
* Axios NPM パッケージを悪用したサプライチェーン
    * https://socket.dev/blog/axios-npm-package-compromised
    * https://www.darkreading.com/application-security/axios-npm-package-compromised-precision-attack
    * https://securityboulevard.com/2026/03/axios-hijacked-npm-account-takeover-deploys-cross-platform-rat-to-millions/

# 攻撃、脅威

* WhatsApp 経由のVBS配布についてMSが警告
    * https://thehackernews.com/2026/04/microsoft-warns-of-whatsapp-delivered.html

# 脆弱性

* CVE-2026-34714 Vim 細工されたコードを開くとコード実行
    * https://www.security-next.com/182763
    * https://cvemon.intruder.io/cves/CVE-2026-34714
    * https://gbhackers.com/claude-ai-zero-day-rce-vulnerabilities-in-vim-and-emacs/
* CVE-2025-53521 F5 BIG-IP 新たにRCEの可能性が浮上し、CVSS見直し
    * https://my.f5.com/manage/s/article/K000156741
    * https://www.darkreading.com/application-security/f5-big-ip-vulnerability-reclassified-rce-exploitation
    * https://www.securityweek.com/f5-big-ip-dos-flaw-upgraded-to-critical-rce-now-exploited-in-the-wild/
* CVE-2026-27876 Grafana RCE
    * https://gbhackers.com/critical-grafana-flaws/

## KEV
* CVE-2026-3502 TrueConf Client Download of Code Without Integrity Check Vulnerability 
* CVE-2026-5281 Google Dawn Use-After-Free Vulnerability

# その他
* macOS CrickFix に対する対策を追加か？警告画面が出る報告
    * https://www.bleepingcomputer.com/news/security/apple-adds-macos-terminal-warning-to-block-clickfix-attacks/
    * https://www.theregister.com/2026/03/31/whatsapp_message_bad_msi_packages/
    * https://gbhackers.com/apple-adds-clickfix-attack-warnings-in-new-macos-tahoe/
* Microsoft Teams  EXIF の削除を追加
    * https://gbhackers.com/microsoft-teams-exif-data-removal-feature/
