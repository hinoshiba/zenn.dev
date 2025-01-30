---
title: "2025/01/26 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威

# 脆弱性

* CVE-2024-11218 Podman and Buildah コンテナ外へのアクセス
    * https://securityonline.info/podman-and-buildah-vulnerable-to-container-breakout-cve-2024-11218/
* CVE-2025-23040 GitHub Desktop 細工されたURLによる認証情報流出の可能性
    * https://thehackernews.com/2025/01/github-desktop-vulnerability-risks.html
* CVE-2025-24085 Apple iOSデバイス。権限昇格の脆弱性。ゼロデイ
    * https://www.bleepingcomputer.com/news/security/apple-fixes-this-years-first-actively-exploited-zero-day-bug/
    * https://www.darkreading.com/endpoint-security/apple-patches-actively-exploited-zero-day-vulnerability
    * https://securityonline.info/cve-2025-24085-apple-patches-actively-exploited-zero-day-vulnerability/
* 昨年末に公開された、CVE-2024-56626 & CVE-2024-56627 Linux SMBに関する脆弱性、PoCリリース
    * https://securityonline.info/cve-2024-56626-cve-2024-56627-critical-linux-kernel-smb-server-bugs-uncovered-poc-published/
* AppleデバイスのCPUに関するサイドチャネル攻撃「SLAP」と「FLOP」
    * https://www.securityweek.com/new-slap-and-flop-cpu-attacks-expose-data-from-apple-computers-phones/
    * https://thehackernews.com/2025/01/new-slap-flop-attacks-expose-apple-m.html
* CVE-2025-0065 TeamViewer 権限昇格の脆弱性
    * https://www.security-next.com/166680
* CVE-2025-22218 VMware Aria Operations および、VMware Cloud Foundation。閲覧権限のみのアカウントで、管理対象の製品の認証情報を閲覧できる可能性
    * https://www.securityweek.com/vmware-patches-high-risk-flaws-in-oft-targeted-aria-operations-products/
* CVE-2024-12647 Canon プリンタ 遠隔からのコード実行の脆弱性
    * https://securityonline.info/cve-2024-12647-cvss-9-8-canon-printers-at-risk-of-remote-code-execution/

## KEV
* CVE-2025-24085 Apple Multiple Products Use-After-Free Vulnerability


# その他
* Google Chrome 2025年の早いうちに、古いChromeでのGoogle Syncが無効となる変更を予定
    * https://www.bleepingcomputer.com/news/google/google-to-kill-chrome-sync-on-older-chrome-browser-versions/
* Signal 新しいデバイスを追加した際に、メッセージをsyncできる機能を追加
    * https://www.bleepingcomputer.com/news/security/signal-will-let-you-sync-old-messages-when-linking-new-devices/
