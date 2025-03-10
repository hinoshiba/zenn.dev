---
title: "2025/03/02 週 セキュリティニュースメモ"
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

* NTTコムにサイバー攻撃 - 法人顧客情報が流出した可能性
    * https://www.security-next.com/167889

# 攻撃、脅威

# 脆弱性

* CVE-2025-27110 ModSecurity ルールのbypassの脆弱性
    * https://securityonline.info/cve-2025-27110-modsecurity-vulnerability-leaves-web-applications-exposed/
* CVE-2025-22224 VMware ESXi, vSphere, Workstation, Fusion, Cloud Foundation, and Telco Cloud Platform 権限昇格の脆弱性
    * https://www.theregister.com/2025/03/04/vmware_plugs_three_hypervisorhijack_holes/
    * https://thehackernews.com/2025/03/vmware-security-flaws-exploited-in.html
    * https://www.bleepingcomputer.com/news/security/broadcom-fixes-three-vmware-zero-days-exploited-in-attacks/
    * https://www.bleepingcomputer.com/news/security/over-37-000-vmware-esxi-servers-vulnerable-to-ongoing-attacks/
* CVE-2024-43093 Android 権限昇格の脆弱性 ゼロデイ
    * https://www.bleepingcomputer.com/news/security/google-fixes-android-zero-days-exploited-in-targeted-attacks/
    * https://securityonline.info/android-alert-critical-flaws-cve-2024-43093-cve-2024-50302-exploited-update-now/
* CVE-2025-0159 IBM Storage 認証Bypassの脆弱性
    * https://securityonline.info/cve-2025-0159-cvss-9-1-critical-ibm-storage-flaw-allows-authentication-bypass/
* CVE-2025-23388 Rancher DoSの脆弱性
    * https://securityonline.info/flaws-in-rancher-cve-2025-23388-cve-2025-23389-expose-kubernetes-environments-to-attacks/
* 2月に修正されたHyper-Vの脆弱性 CVE-2025-21333、PoCリリース
    * https://securityonline.info/windows-hyper-v-zero-day-cve-2025-21333-poc-drops-system-access-exposed/
* CVE-2025-25015 Kibana RCE
    * https://securityonline.info/cve-2025-25015-cvss-9-9-critical-code-execution-vulnerability-patched-in-elastic-kibana/
* CVE-2025-1080 LibreOffice スクリプトの実行
    * https://securityonline.info/cve-2025-1080-libreoffice-patches-security-flaw-allowing-arbitrary-script-execution/
* CVE-2025-27423 Vim 細工されたTarファイルによるスクリプト実行の可能性
    * https://securityonline.info/vim-users-warned-crafted-tar-files-could-trigger-code-execution-cve-2025-27423/

## KEV
* CVE-2023-20118 Cisco Small Business RV Series Routers Command Injection Vulnerability
* CVE-2022-43939 Hitachi Vantara Pentaho BA Server Authorization Bypass Vulnerability
* CVE-2022-43769 Hitachi Vantara Pentaho BA Server Special Element Injection Vulnerability
* CVE-2018-8639 Microsoft Windows Win32k Improper Resource Shutdown or Release Vulnerability
* CVE-2024-4885 Progress WhatsUp Gold Path Traversal Vulnerability

# その他

* Firefox 縦タブリリース
    * https://www.theregister.com/2025/03/04/firefox_136/
* o365 認証周りの障害 3/1 現在は復旧ずみ
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-links-recent-microsoft-365-outage-to-buggy-update/
