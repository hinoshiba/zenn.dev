---
title: "2024/12/08 週 セキュリティニュースメモ"
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

* Microsoft365 管理センター等に障害
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-365-outage-takes-down-office-web-apps-admin-center/
    * https://x.com/MSFT365Status/status/1866439364932251718

# 攻撃、脅威

# 脆弱性

* CVE-2024-12209 WordPress Plugin Umbrella 未認証のアクセスの脆弱性
    * https://securityonline.info/cve-2024-12209-cvss-9-8-wp-umbrella-plugin-vulnerability-exposes-30000-websites-to-compromise/
    * https://rocket-boys.co.jp/11257/
* 8月に修正されたWindows脆弱性、PoCリリース CVE-2024-38193
    * https://securityonline.info/windows-zero-day-vulnerability-cve-2024-38193-exploited-in-the-wild-poc-published/
* CVE-2024-48863 QNAP 任意のコード実行の脆弱性
    * https://securityonline.info/qnap-addresses-high-severity-vulnerabilities-in-license-center-and-operating-systems/
* CVE-2024-39343 and CVE-2024-53842 Google Pixel RCE
    * https://securityonline.info/google-fixes-critical-rce-vulnerabilities-in-december-2024-pixel-security-update/
* CVE-2024-11205 WordPress Plugin WPForm 任意の払い戻し実行やキャンセルの実行
    * https://www.bleepingcomputer.com/news/security/wpforms-bug-allows-stripe-refunds-on-millions-of-wordpress-sites/
    * https://securityonline.info/cve-2024-11205-wpforms-plugin-vulnerability-impacts-6-million-wordpress-sites/
* CVE-2024-11639 Ivanti CSA 遠隔からの認証bypassによる管理権限アクセス
    * https://www.bleepingcomputer.com/news/security/ivanti-warns-of-maximum-severity-csa-auth-bypass-vulnerability/
    * https://www.security-next.com/165155
* CVE-2024-47578 SAP NetWeaver AS for JAVA 他脆弱性との組み合わせで、任意のコード実行の可能性
    * https://securityonline.info/cve-2024-47578-cvss-9-1-sap-issues-critical-patch-for-netweaver-as-for-java/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Dec
        * https://msrc.microsoft.com/blog/2024/12/202412-security-update/
        * https://www.theregister.com/2024/12/10/microsoft_patch_tuesday/
        * https://www.securityweek.com/microsoft-ships-urgent-patch-for-exploited-windows-clfs-zero-day/
        * https://www.cisa.gov/news-events/alerts/2024/12/10/microsoft-releases-december-2024-security-updates
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-december-2024-patch-tuesday-fixes-1-exploited-zero-day-71-flaws/
        * https://www.bleepingcomputer.com/news/microsoft/windows-11-kb5048667-and-kb5048685-cumulative-updates-released/
        * https://www.bleepingcomputer.com/news/microsoft/windows-10-kb5048652-update-fixes-new-motherboard-activation-bug/

## KEV
* CVE-2024-49138 Microsoft Windows Common Log File System (CLFS) Driver Heap-Based Buffer Overflow Vulnerability

# その他

* JPCERT/CC インシデント報告Webフォームメンテナンス 2024年12月19日（木）9:00 - 15:00
    * https://www.jpcert.or.jp/maintenance20241209.html
* Cloudflare 2024年レビュー
    * https://blog.cloudflare.com/radar-2024-year-in-review/
* Mandiant社、QRコードによるC2通信のPoCを公開
    * https://www.bleepingcomputer.com/news/security/qr-codes-bypass-browser-isolation-for-malicious-c2-communication/
    * https://www.darkreading.com/endpoint-security/attackers-qr-codes-bypass-browser-isolation
* デフォルト設定のNTLMリレー軽減
    * https://msrc.microsoft.com/blog/2024/12/mitigating-ntlm-relay-attacks-by-default-ja/
* Lets Encrypt OCSPから、CRLへの移行。2025年8月までの予定
    * https://securityonline.info/lets-encrypt-to-deprecate-ocsp-in-favor-of-crls-enhancing-user-privacy/
