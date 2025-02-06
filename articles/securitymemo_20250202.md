---
title: "2025/02/02 週 セキュリティニュースメモ"
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
* Cacio UK オンラインストア Javascript埋め込みによりクレジットカード情報等が盗まれた可能性
    * https://www.bleepingcomputer.com/news/security/casio-uk-online-store-hacked-to-steal-customer-credit-cards/
    * https://news.mynavi.jp/techplus/article/20250205-3122269/


# 脆弱性

* CVE-2024-53104 Android 権限昇格の脆弱性 ゼロデイ
    * https://securityonline.info/cve-2024-53104-critical-zero-day-vulnerability-patched-in-february-2025-android-security-update/
    * https://www.bleepingcomputer.com/news/security/google-fixes-android-kernel-zero-day-exploited-in-attacks/
* CVE-2025-24118 Appleデバイス。メモリプロテクション管理
    * https://securityonline.info/poc-exploit-released-for-macos-kernel-vulnerability-cve-2025-24118-cvss-9-8/
* PSV-2023-0039 Netgear ルータ、未認証のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/netgear-warns-users-to-patch-critical-wifi-router-vulnerabilities/
* CVE-2025-21293 2025/01に修正されたADの権限昇格の脆弱性、PoCリリース
    * https://securityonline.info/privilege-escalation-in-active-directory-domain-services-cve-2025-21293-exploit-revealed-with-poc-code/
* CVE-2024-56161 AMDのCPU マイクロコード挿入の脆弱性
    * https://www.bleepingcomputer.com/news/security/amd-fixes-bug-that-lets-hackers-load-malicious-microcode-patches/
* CVE-2025-20124 Cisco ISE 遠隔からのコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/critical-cisco-ise-bug-can-let-attackers-run-commands-as-root/
    * https://securityonline.info/cve-2025-20124-cve-2025-20125-cisco-patches-critical-flaws-in-identity-services-engine/
* CVE-2025-23419 NGINX クライアントの認証をbypassできる脆弱性
    * https://securityonline.info/f5-warns-of-tls-session-resumption-vulnerability-in-nginx-cve-2025-23419/
* CVE-2025-24503 Symantec PAM コード実行の脆弱性
    * https://securityonline.info/symantec-pam-patches-critical-security-flaw-cve-2025-24503-cvssv4-9-3/

## KEV
* CVE-2024-53104 Linux Kernel Out-of-Bounds Write Vulnerability
* CVE-2025-0411 7-Zip Mark of the Web Bypass Vulnerability
* CVE-2022-23748 Dante Discovery Process Control Vulnerability
* CVE-2024-21413 Microsoft Outlook Improper Input Validation Vulnerability
* CVE-2020-29574 CyberoamOS (CROS) SQL Injection Vulnerability
* CVE-2020-15069 Sophos XG Firewall Buffer Overflow Vulnerability


# その他
* 「サイバーセキュリティ月間」がスタート - チョコプラ「TT兄弟」も登場
    * https://www.security-next.com/166817
* 【イギリス】政府、「AIサイバーセキュリティ行動規範」発表。
    * https://sustainablejapan.jp/2025/02/02/uk-ai-cyber-security-code-of-practice/110396
* Microsoft Defender VPN 2/28 で終了
    * https://www.darkreading.com/mobile-security/microsoft-sets-end-date-for-defender-vpn
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-kills-off-defender-privacy-protection-vpn-feature/
* WSL2 Arch Linux をサポート
    * https://securityonline.info/arch-linux-on-wsl-2-microsoft-confirms-official-support/
