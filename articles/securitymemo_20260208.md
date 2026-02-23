---
title: "2026/02/08 週 セキュリティニュースメモ"
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

* JAL / 「手荷物当日配送サービス」予約システムへの不正アクセスについて
    * https://www.jal.co.jp/jp/ja/info/2026/other/260210/
    * 原因は誤操作で不正アクセスではなかった
    * https://xtech.nikkei.com/atcl/nxt/column/18/00001/11510/
* Gala湯沢 / 弊社サーバーへの不正アクセスによりお客さま情報が漏えいした可能性について
    * https://gala.co.jp/winter/pickup/60429/
        * `2020 年12 月 16 日から 2026 年２月１日までGALAシーズンパスポートをご購入されたお客さまの個人情報 最大 1,518 名分`

# 攻撃、脅威

# 脆弱性

* CVE-2026-21643 FortiClient EMS SQLi
    * https://thehackernews.com/2026/02/fortinet-patches-critical-sqli-flaw.html
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-feb
        * https://cybersecuritynews.com/microsoft-patch-tuesday-february-2026/
        * https://krebsonsecurity.com/2026/02/patch-tuesday-february-2026-edition/
        * https://gbhackers.com/microsoft-patch-tuesday-february-2026-fixes-54-flaws/
    * CVE-2026-21533 Windows Remote Desktop Services EoP
        * https://cybersecuritynews.com/windows-remote-desktop-services-0-day-vulnerability/
    * CVE-2026-20841 Notepad Code Execuion
        * https://cvemon.intruder.io/cves/CVE-2026-20841
        * https://x.com/co11ateral/status/2021544437889867825
        * https://www.bleepingcomputer.com/news/microsoft/windows-11-notepad-flaw-let-files-execute-silently-via-markdown-links/
    * CVE-2026-21514 Word セキュリティ機能の回避
        * https://gbhackers.com/microsoft-office-word-0-day-vulnerability/
* CVE-2025-7659 GitLab IDE 未認証のアクセス
    * https://cvemon.intruder.io/cves/CVE-2025-7659
    * https://securityonline.info/gitlab-patch-alert-high-severity-web-ide-flaw-exposes-private-repos/
* CVE-2026-1357 WordPress WPvivid Backup & Migration plugin RCE
    * https://www.bleepingcomputer.com/news/security/wordpress-plugin-with-900k-installs-vulnerable-to-critical-rce-flaw/
    * https://gbhackers.com/wordpress-backup-plugin-vulnerability/
* CVE-2026-20700 Apple Device コード実行の脆弱性
    * https://www.securityweek.com/apple-patches-ios-zero-day-exploited-in-extremely-sophisticated-attack/
    * https://thehackernews.com/2026/02/apple-fixes-exploited-zero-day.html
    * https://gbhackers.com/apple-0-day-flaw-actively-exploited/

## KEV

# その他
* Firefox AI機能を一括無効化するボタンを追加
    * https://news.mynavi.jp/techplus/article/20260208-4083211/
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/firefox-ai-kill-switch
* Bitwarden チームパスワードシェア機能 / Cupid Vault
    * https://www.bleepingcomputer.com/news/security/bitwarden-introduces-cupid-vault-for-secure-password-sharing/
