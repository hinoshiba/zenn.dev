---
title: "2025/03/30 週 セキュリティニュースメモ"
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

* CVE-2025-1268 Canon Printer コード実行の可能性
    * https://securityonline.info/canon-fixes-critical-printer-driver-flaw-cve-2025-1268-alert/
    * https://www.securityweek.com/critical-vulnerability-found-in-canon-printer-drivers/
* CVE-2025-2825 CrushFTP 認証bypassの脆弱性
    * https://securityonline.info/crushftp-hacked-exploit-cve-2025-2825-with-poc-and-nuclei-template/
    * https://securityboulevard.com/2025/04/exploited-critical-unauthenticated-access-vulnerability-in-crushftp-cve-2025-2825/
    * https://www.bleepingcomputer.com/news/security/critical-auth-bypass-bug-in-crushftp-now-exploited-in-attacks/
* CVE-2025-30095 VyOS MITM
    * https://securityonline.info/vyos-and-debian-systems-vulnerable-to-man-in-the-middle-attacks-cve-2025-30095/
* CVE-2025-30223 Beego XSS
    * https://securityonline.info/cve-2025-30223-cvss-9-3-critical-xss-vulnerability-discovered-in-beego-framework/
* CVE-2025-30065 Apache Parquet Java Arbitrary Code Execution
    * https://securityonline.info/cve-2025-30065-cvss-10-critical-vulnerability-discovered-in-apache-parquet-java/
    * https://www.bleepingcomputer.com/news/security/max-severity-rce-flaw-discovered-in-widely-used-apache-parquet/
* Apple Backports Critical Fixes for 3 Recent 0-Days
    * https://thehackernews.com/2025/04/apple-backports-critical-fixes-for-3.html
    * https://www.securityweek.com/apple-patches-recent-zero-days-in-older-iphones/
* CVE-2025-27095 JumpServer Token流出の可能性
    * https://securityonline.info/cve-2025-27095-token-theft-flaw-in-jumpserver-exposes-kubernetes-clusters-to-unauthorized-access/
* CVE-2025-22457 Ivanti Connect Secure RCE
    * https://www.bleepingcomputer.com/news/security/ivanti-patches-connect-secure-zero-day-exploited-since-mid-march/
    * https://securityonline.info/cve-2025-22457-unc5221-exploits-ivanti-zero-day-flaw-to-deploy-trailblaze-and-brushfire-malware/
* CVE-2025-31334 WinRAR MotW Bypass
    * https://securityonline.info/cve-2025-31334-winrar-flaw-enables-mark-of-the-web-bypass-and-arbitrary-code-execution/
* CVE-2025-31720 Jenkins 認可不備による機密情報窃取
    * https://securityonline.info/multiple-jenkins-plugin-and-core-vulnerabilities-expose-sensitive-data-and-execution-paths/
* CVE-2025-23391 Rancher より強い管理者権限の奪取
    * https://securityonline.info/rancher-users-update-now-to-fix-admin-takeover-bug-cve-2025-23391/


## KEV
* CVE-2024-20439 Cisco Smart Licensing Utility Static Credential Vulnerability
* CVE-2025-24813 Apache Tomcat Path Equivalence Vulnerability
    * https://securityonline.info/cisa-flags-apache-tomcat-cve-2025-24813-as-actively-exploited-with-9-8-cvss/

# その他

* Ubuntu セキュリティ機能のバイパスに対する手動の対策
    * https://www.bleepingcomputer.com/news/security/new-ubuntu-linux-security-bypasses-require-manual-mitigations/
* Androidパスワードマネージャ、Passkey対応
    * https://securityonline.info/google-password-manager-adds-passkeys-future-export-teased/
* IPA 企業向けセキュリティ相談窓口を開設
    * https://www.ipa.go.jp/security/support/soudan.html
