---
title: "2024/07/14 週 セキュリティニュースメモ"
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
* Disny 1.1TB のデータが盗まれた可能性
    * https://www.bitdefender.com/blog/hotforsecurity/disney-hacked-nullbulge-1-1-tb-data-internal-slack/
    * https://www.cnn.co.jp/business/35221520.html
    * https://securityboulevard.com/2024/07/disney-nullbulge-slack-hack-richixbw/
    * https://news.mynavi.jp/techplus/article/20240717-2987418/
* イセトー、ランサムウェア被害。和歌山市等
   * https://www.mbs.jp/news/kansainews/20240716/GE00058909.shtml   
   * https://scan.netsecurity.ne.jp/article/2024/07/17/51316.html 
* 東京ガスや子会社で個人情報流出の可能性 - 約416万人分
    * https://www.security-next.com/159799
    * https://news.google.com/rss/articles/CBMiR2h0dHBzOi8vYXJ0aWNsZS5hdW9uZS5qcC9kZXRhaWwvMS8zLzYvNDA3XzZfcl8yMDI0MDcxN18xNzIxMjA1MDYxNzE4MzA40gEA?oc=5

# 脆弱性

* CVE-2024-6387 RegreSSH Windowsには影響ないとMicrosoftアドバイザリにて
    * https://www.securityweek.com/microsoft-says-windows-not-impacted-by-regresshion-as-second-openssh-bug-is-found/
    * https://msrc.microsoft.com/update-guide/vulnerability/CVE-2024-6387
* CVE-2024-36435 Supermicro BMC RCE
    * https://securityonline.info/supermicro-motherboards-vulnerable-to-critical-rce-flaw-cve-2024-36435/
* CVE-2024-36401 GeoServer Critial RCE Attack PoC公開
    * https://securityonline.info/cve-2024-36401-cvss-9-8-critical-geoserver-flaw-under-active-attack-poc-available/
    * https://www.bleepingcomputer.com/news/security/cisa-warns-critical-geoserver-geotools-rce-flaw-is-exploited-in-attacks/
    * https://thehackernews.com/2024/07/cisa-warns-of-actively-exploited-rce.html
* CVE-2024-20419 Cisco SSM 未認証のパスワード変更の脆弱性
   * https://securityvulnerability.io/vulnerability/CVE-2024-20419  
   * https://securityonline.info/cve-2024-20419-cvss-10-critical-flaw-in-cisco-smart-software-manager-opens-door-to-account-takeover/
   * https://www.bleepingcomputer.com/news/security/cisco-ssm-on-prem-bug-lets-hackers-change-any-users-password/
* CVE-2024-20435 Cisco AsyncOS 任意のコード実行の脆弱性
   * https://vulners.com/nvd/NVD:CVE-2024-20435  
* CVE-2024-20401 Cisco Secure Email Gateway 未認証のファイルアップロードの脆弱性
   * https://vulners.com/nvd/NVD:CVE-2024-20401   
   * https://securityonline.info/critical-security-flaw-in-cisco-secure-email-gateway-cve-2024-20401/
* CVE-2024-3738 Ivanti EPM SQLi
    * https://securityonline.info/ivanti-patches-sqli-vulnerability-cve-2024-37381-in-endpoint-management-software/
    * https://securityonline.info/ivanti-patches-sqli-vulnerability-cve-2024-37381-in-endpoint-management-software/
* CVE-2024-27348 Apache HugeGraph RCE
    * https://thehackernews.com/2024/07/critical-apache-hugegraph-vulnerability.html 
* CVE-2024-4143 HP AMI BIOS 権限昇格の脆弱性
    * https://www.tenable.com/cve/CVE-2024-4143   
* CVE-2024-6695 WordPress Plugin Profile Builder 管理者権限の窃取
   * https://wpscan.com/blog/unauthenticated-privilege-escalation-in-profile-builder-plugin/
   * https://securityonline.info/cve-2024-6695-cvss-9-8-in-popular-wordpress-plugin-exposes-50000-sites-to-admin-hijacking/ 
* KEV
    * CVE-2024-36401 GeoServer GeoTools Eval Injection Vulnerability
    * CVE-2024-34102 Adobe Commerce and Magento Open Source Improper Restriction of XML External Entity Reference (XXE) Vulnerability
    * CVE-2024-28995 SolarWinds Serv-U Path Traversal Vulnerability
    * CVE-2022-22948 VMware vCenter Server Incorrect Default File Permissions Vulnerability

# その他
* Google(Alphabet) サイバーセキュリティ企業Wizを買収の動き
    * https://securityonline.info/alphabet-to-acquire-cybersecurity-powerhouse-wiz-for-23-billion/
* ハッカーはPoCが公開されてから22分後に攻撃を始める Cloudflare reportより
    * https://www.bleepingcomputer.com/news/security/hackers-use-poc-exploits-in-attacks-22-minutes-after-release/
    * https://blog.cloudflare.com/application-security-report-2024-update
* 能動的サイバー防御、メタ情報を第三者が監視の方向で検討
    * https://jp.inoreader.com/article/3a9c6e74795ed544-
* カスペルスキー、7/20をもって、アメリカでのビジネスを終了
    * https://www.bleepingcomputer.com/news/security/kaspersky-is-shutting-down-its-business-in-the-united-states/
    * https://thehackernews.com/2024/07/kaspersky-exits-us-market-following.html
    * https://news.mynavi.jp/techplus/article/20240716-2986527/
    * https://www.theregister.com/2024/07/17/kaspersky_goodbye_gift/
 * WindowsServer 6月の更新によってDefenderの機能に不具合
   * https://www.bleepingcomputer.com/news/microsoft/june-windows-server-updates-break-microsoft-365-defender-features/ 
* Cloudflare アプリケーションセキュリティレポート公開
    * https://blog.cloudflare.com/application-security-report-2024-update
    * https://news.google.com/rss/articles/CBMiQmh0dHBzOi8vd3d3Lml0bWVkaWEuY28uanAvZW50ZXJwcmlzZS9hcnRpY2xlcy8yNDA3LzE3L25ld3MwNTcuaHRtbNIBAA
* Exchange Online adds Inbound DANE
    * https://www.bleepingcomputer.com/news/microsoft/exchange-online-adds-inbound-dane-with-dnssec-for-security-boost/ 