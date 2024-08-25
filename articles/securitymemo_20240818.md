---
title: "2024/08/18 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
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

* セイコーエプソン 不正アクセス。現時点で流出は確認されていない
    * https://corporate.epson/ja/news/2024/240808.html
    * https://scan.netsecurity.ne.jp/article/2024/08/14/51470.html
* 機密データへの不正アクセスを防止・報告しなかったとしてT-Mobileに80億円超の罰金
    * https://gigazine.net/news/20240817-cfius-tmobile-60-million-usd-penalty/
* Toyota アメリカ支社から240GiBデータ流出
    * https://www.bleepingcomputer.com/news/security/toyota-confirms-third-party-data-breach-impacting-customers/
    * https://gigazine.net/news/20240820-toyota-stolen-data-leaks/
* ニデックプレシジョン株式会社 ベトナム子会社にサイバー攻撃。身代金要求
    * https://www.nidec.com/jp/nidec-precision/corporate/news/2024%E5%B9%B4/20240812_%20incident/
    * https://cybersecurity-jp.com/news/98810
* 豊田市 約15万人に影響 イセトーへのサイバー攻撃関連
    * https://www.nagoyatv.com/news/?id=025951
    * https://www3.nhk.or.jp/tokai-news/20240820/3000037048.html
* Netflix 未公開のエピソードに関する情報がインターネット上に流出。セキュリティ上の問題
    * https://www.bitdefender.com/blog/hotforsecurity/hacker-leaks-upcoming-episodes-of-netflix-shows-online-following-security-breach/

# 脆弱性
* macOS上で動作するOfficeソフトに、ライブラリインジェクションの脆弱性があるとCiscoTalosリサーチャ報告。Microsoftは修正予定無しとのこと
    * https://www.darkreading.com/remote-workforce/multiple-microsoft-apps-for-macos-vuln-to-malicious-library-injection-attacks
    * https://www.theregister.com/2024/08/19/cisco_talos_microsoft_macos/
    * https://www.securityweek.com/cisco-microsoft-disagree-on-severity-of-macos-app-vulnerabilities/
* CVE-2024-7646 k8s ingress-nginx 認証bypass
    * https://securityonline.info/cve-2024-7646-a-threat-to-kubernetes-clusters-running-ingress-nginx/
* CVE-2024-30949 RISC-V newlibの除算誤りによる任意のコード実行
    * https://inbox.sourceware.org/newlib/20231129035714.469943-1-visitorckw%40gmail.com/
    * https://access.redhat.com/security/cve/cve-2024-30949
* CVE-2024-39809 BIG-IP Next Central Manager ログアウト後にもセッションが破棄されない脆弱性。管理コンソールのみ
    * https://www.securityweek.com/f5-patches-high-severity-vulnerabilities-in-big-ip-nginx-plus/
    * https://securityonline.info/f5-issues-security-advisories-for-nginx-plus-cve-2024-39792-big-ip-next-central-manager-cve-2024-39809/
* CVE-2024-39778 BIG-IP 未認証のユーザによるDoSの脆弱性
    * https://www.securityweek.com/f5-patches-high-severity-vulnerabilities-in-big-ip-nginx-plus/
    * https://securityonline.info/f5-issues-security-advisories-for-nginx-plus-cve-2024-39792-big-ip-next-central-manager-cve-2024-39809/
* CVE-2024-5932 WordPress Plugin GiveWP 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-5932-cvss-10-critical-rce-vulnerability-impacts-100k-wordpress-sites/
    * https://www.bitdefender.com/blog/hotforsecurity/over-100-000-wordpress-websites-vulnerable-to-takeover-due-to-critical-donation-plugin-flaw/
    * https://thehackernews.com/2024/08/givewp-wordpress-plugin-vulnerability.html
    * https://www.security-next.com/160981
* CVE-2024-7971 Google Chrome 任意のコード実行やブラウザクラッシュの可能性
    * https://www.bleepingcomputer.com/news/security/google-fixes-tenth-actively-exploited-chrome-zero-day-in-2024/
    * https://www.darkreading.com/vulnerabilities-threats/google-chrome-update-fixes-flaw-exploited-in-the-wild
    * https://www.bleepingcomputer.com/news/security/google-fixes-ninth-actively-exploited-chrome-zero-day-in-2024/
* CVE-2024-28000 WordPress Plugin LiteSpeedCache 未認証の管理者権限
    * https://www.bleepingcomputer.com/news/security/litespeed-cache-bug-exposes-millions-of-wordpress-sites-to-takeover-attacks/
    * https://securityonline.info/cve-2024-28000-active-exploitation-litespeed-cache-vulnerability/
    * https://securityonline.info/cve-2024-28000-in-litespeed-cache-plugin-actively-exploited-over-30000-attacks-blocked-in-24-hours/
    * https://www.bleepingcomputer.com/news/security/hackers-are-exploiting-critical-bug-in-litespeed-cache-plugin/
* CVE-2024-6800 GitHub Enterprise 管理者への権限昇格の脆弱性
    * https://www.securityweek.com/critical-authentication-flaw-haunts-github-enterprise-server/
    * https://www.bleepingcomputer.com/news/security/github-enterprise-server-vulnerable-to-critical-auth-bypass-flaw/
    * https://securityonline.info/cve-2024-6800-cvss-9-5-critical-github-enterprise-server-flaw-patched-admin-access-at-risk/
    * https://www.security-next.com/160998
    * https://thehackernews.com/2024/08/github-patches-critical-security-flaw.html
* CVE-2024-38021 7月に修正されたOutlookのゼロクリック攻撃、PoC公開
    * https://securityonline.info/researcher-details-microsoft-outlook-zero-click-vulnerability-cve-2024-38021/
* CVE-2024-7272 FFmpeg ヒープオーバーフロー PoC公開
    * https://securityonline.info/cve-2024-7272-critical-heap-overflow-vulnerability-discovered-in-ffmpeg-poc-published/
* CVE-2024-38810 Spring Framework 未認証のアクセス
    * https://securityonline.info/cve-2024-38810-spring-security-flaw-leaves-applications-open-to-unauthorized-access/
* CVE-2024-21689 Atlassian Bamboo Data Center RCE
    * https://securityonline.info/cve-2024-21689-rce-vulnerability-in-atlassian-bamboo-data-center-and-server/
* KEV
    * CVE-2021-33044 Dahua IP Camera Authentication Bypass Vulnerability
    * CVE-2021-33045 Dahua IP Camera Authentication Bypass Vulnerability
    * CVE-2022-0185 Linux Kernel Heap-Based Buffer Overflow
    * CVE-2021-31196 Microsoft Exchange Server Information Disclosure Vulnerability
    * CVE-2024-23897 Jenkins Command Line Interface (CLI) Path Traversal Vulnerability
        * https://www.bleepingcomputer.com/news/security/cisa-warns-of-jenkins-rce-bug-exploited-in-ransomware-attacks/
        * https://www.security-next.com/160926

# その他
* Windows11 24H2 より、BitLockerがデフォルトに。
    * https://securityonline.info/windows-11-24h2-microsoft-enforces-device-encryption-by-default/
* Teams(unified teams app) 複数アカウントのスイッチに対応
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-launches-unified-teams-app-for-personal-work-accounts/
* 8月のWindowsUpdateによりデュアルブート環境に不具合。Linux等が起動せず。
    * https://www.bleepingcomputer.com/news/microsoft/august-windows-updates-break-dual-boot-on-some-linux-systems/
    * https://www.theregister.com/2024/08/21/microsoft_patch_dual_boot/
    * https://www.bleepingcomputer.com/news/microsoft/august-windows-security-update-breaks-dual-boot-on-linux-systems/
    * https://securityboulevard.com/2024/08/microsoft-linux-duel-boot-fail-richixbw/
    * 修正や対応、ワークアラウンド
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-confirms-august-updates-break-linux-boot-in-dual-boot-systems/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-shares-temp-fix-for-linux-boot-issues-on-dual-boot-systems/
* Windows Recall 10月にプレビュー公開。セキュリティ懸念への対応もされる予定。詳細は公開時に合わせて情報公開予定
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-roll-out-windows-recall-to-insiders-in-october/
    * https://www.theregister.com/2024/08/22/microsoft_recall_redux/
* Windows 11 コントロールパネルの削除が開始。25H2から段階的に。
    * https://securityonline.info/microsoft-signals-end-of-an-era-control-panel-to-be-phased-out/
