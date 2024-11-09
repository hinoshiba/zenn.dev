---
title: "2024/11/03 週 セキュリティニュースメモ"
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

* ウエルシア薬局 従業員のPCが不正アクセス受け、約4万人分の情報漏洩か
    * https://times.abema.tv/articles/-/10150404?page=1

# 脆弱性

* Okta 認証bypassの不具合を修正。ユーザ名が52文字以上だとハッシュの生成にパスワードを用いない問題
    * https://www.darkreading.com/vulnerabilities-threats/okta-fixes-auth-bypass-bug-three-month-lull
    * https://scan.netsecurity.ne.jp/article/2024/11/06/51863.html
* CVE-2024-9191 Okta Verify Desktop MFA for Windows パスワードやユーザ名が盗まれる脆弱性
    * https://securityonline.info/okta-patches-vulnerability-cve-2024-9191-in-verify-desktop-mfa-for-windows/
    * https://www.security-next.com/163892
* CVE-2024-9162 WordPress Plugin All-in-One WP Migration and Backup 任意のコード実行の脆弱性
    * https://scan.netsecurity.ne.jp/article/2024/11/06/51871.html
* CVE-2024-20418 Cisco URWB 任意のコード実行と管理者権限への昇格の脆弱性
    * https://www.bleepingcomputer.com/news/security/cisco-bug-lets-hackers-run-commands-as-root-on-uwrb-access-points/
    * https://securityonline.info/cve-2024-20418-cvss-10-cisco-urwb-access-points-vulnerable-to-remote-takeover/
    * https://www.theregister.com/2024/11/07/cisco_uiws_flaw/
* CVE-2024-44258 iOS symbolic linkに関する不具合。バックアップ時に影響
    * https://securityonline.info/poc-exploit-releases-for-critical-symlink-flaw-in-apples-ios-cve-2024-44258/
    * https://www.itmedia.co.jp/enterprise/articles/2411/08/news093.html
* CVE-2024-47461 HPE Aruba Networking access points 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/hpe-warns-of-critical-rce-flaws-in-aruba-networking-access-points/
* CVE-2024-10470 WordPress Theme パスとラバーサルの脆弱性
    * https://securityonline.info/cve-2024-10470-cvss-9-8-in-popular-wordpress-theme-exposes-thousands-of-sites/
* CVE-2024-10914 D-Link 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/d-link-wont-fix-critical-flaw-affecting-60-000-older-nas-devices/

## KEV
* CVE-2024-8957 PTZOptics PT30X-SDI/NDI Cameras OS Command Injection Vulnerability
* CVE-2024-8956 PTZOptics PT30X-SDI/NDI Cameras Authentication Bypass Vulnerability
* CVE-2024-43093 Android Framework Privilege Escalation Vulnerability
* CVE-2024-51567 CyberPanel Incorrect Default Permissions Vulnerability
* CVE-2019-16278 Nostromo nhttpd Directory Traversal Vulnerability
* CVE-2024-5910 Palo Alto Expedition Missing Authentication Vulnerability

# その他
* サイバー法案、年内見送りへ　首相交代で設計議論停滞
    * https://www.hokkaido-np.co.jp/article/1083615/
* WindowsServer 2025 Released
    * https://www.bleepingcomputer.com/news/microsoft/windows-server-2025-released-here-are-the-new-features/
* Google Cloud 2025年末までにMFAを義務化へ
    * https://www.bleepingcomputer.com/news/security/google-cloud-to-make-mfa-mandatory-by-the-end-of-2025/
    * https://thehackernews.com/2024/11/google-cloud-to-enforce-multi-factor.html
* notepadやペイントにて、AI機能が追加
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-notepad-to-get-ai-powered-rewriting-tool-on-windows-11/
    * https://www.theregister.com/2024/11/07/microsoft_ai_notepad_paint/
* Interpolが22,000件の悪意あるIPアドレスを削除
    * https://databreaches.net/2024/11/06/interpols-operation-synergia-ii-took-down-22000-malicious-ip-addresses/
    * https://securityboulevard.com/2024/11/interpol-operation-shuts-down-22000-malicious-servers/
    * https://thehackernews.com/2024/11/interpols-operation-synergia-ii.html
* カナダ、TikTokへ閉鎖命令
    * https://www.bleepingcomputer.com/news/security/canada-orders-tiktok-to-shut-down-over-national-risk-concerns/
