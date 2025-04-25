---
title: "2025/04/20 週 セキュリティニュースメモ"
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

* CVE-2025-42599 Active! mail BOF。IIJメールサービスの原因
    * https://securityonline.info/cve-2025-42599-critical-buffer-overflow-in-active-mail-exploited-in-the-wild/
    * https://rocket-boys.co.jp/security-measures-lab/iij-cyberattack-active-mail-zero-day-cve-2025-42599/
* CVE-2024-54085 ASUS MegaRAC Baseboard Management Controller RCE
    * https://www.bleepingcomputer.com/news/security/asus-releases-fix-for-ami-bug-that-lets-hackers-brick-servers/
* CVE-2025-25427 TP-Link WR841N Router Stored XSS
    * https://securityonline.info/stored-xss-flaw-in-tp-link-wr841n-routers-could-expose-admin-credentials-cve-2025-25427/
* CVE-2025-21204 Windows 今月の月次アップデートで修正された権限昇格の脆弱性PoCリリース
    * https://securityonline.info/cve-2025-21204-system-level-privilege-escalation-in-windows-update-stack-exposed-poc-released/
* CVE-2025-33028 WinZip WotW のBypass
    * https://securityonline.info/cve-2025-33028-winzip-flaw-exposes-users-to-silent-code-execution-via-motw-bypass-no-patch/
    * https://www.security-next.com/169579
* CVE-2025-2492 ASUS ルータ、認証回避の脆弱性
    * https://www.darkreading.com/cloud-security/asus-patch-aicloud-router-vuln
    * https://securityonline.info/cve-2025-2492-critical-asus-router-vulnerability-requires-immediate-firmware-update/
* CVE-2024-53104 Android 権限昇格の脆弱性。ゼロデイ
    * https://securityonline.info/cellebrite-android-zero-day-exploit-poc-released-cve-2024-53104/
* CVE-2025-32434 PyTorch RCE
    * https://securityonline.info/critical-pytorch-vulnerability-cve-2025-32434-allows-remote-code-execution/
* CVE-2025-1763 and CVE-2025-2443  GitLab XSS 
    * https://securityonline.info/gitlab-releases-security-update-to-patch-xss-and-account-takeover-flaws/
* CVE-2025-3260 Grafana 未認証のアクセス
    * https://securityonline.info/grafana-patches-cve-2025-3260-and-more-in-critical-security-update/


# その他

* MITRE CVEの資金調達問題。契約失効前に解決されたとのこと
    * https://securityonline.info/cisa-clarifies-cve-programs-stability-amid-funding-concerns/
    * https://www.cisa.gov/news-events/news/statement-matt-hartman-cve-program
* Linux io_uring セキュリティの盲点によりルートキット攻撃が可能というコンセプト。EDRのカスタムシグネチャでも検知が難しい
    * https://www.bleepingcomputer.com/news/security/linux-io-uring-security-blindspot-allows-stealthy-rootkit-attacks/
    * https://thehackernews.com/2025/04/linux-iouring-poc-rootkit-bypasses.html
