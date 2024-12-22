---
title: "2024/12/15 週 セキュリティニュースメモ"
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

* Juniper がSSRデバイスのデフォルト認証情報を用いたbotネットのターゲットになることを警告
    * https://thehackernews.com/2024/12/juniper-warns-of-mirai-botnet-targeting.html
    * https://www.bleepingcomputer.com/news/security/juniper-warns-of-mirai-botnet-targeting-session-smart-routers/

# 脆弱性

* CVE-2023-34990 Wireless LAN Manager (FortiWLM) 未認証の管理者アクセスの脆弱性
    * https://thehackernews.com/2024/12/fortinet-warns-of-critical-fortiwlm.html
    * https://securityonline.info/cve-2023-34990-cvss-9-8-critical-security-flaw-found-in-fortinet-fortiwlm/
    * https://www.security-next.com/165455
    * https://codebook.machinarecord.com/threatreport/36610/
* CVE-2024-50379 Apache Tomcat RCE
    * https://securityonline.info/rce-and-dos-vulnerabilities-addressed-in-apache-tomcat-cve-2024-50379-and-cve-2024-54677/
    * https://www.security-next.com/165419
    * https://securityboulevard.com/2024/12/cve-2024-50379-a-critical-race-condition-in-apache-tomcat/
    * https://securityboulevard.com/2024/12/apache-tomcat-conditional-competition-code-execution-vulnerability-cve-2024-50379/
* CVE-2024-55661 Laravel Pulse RCE
    * https://www.security-next.com/165404
* CVE-2024-45337 Go言語 認証バイパスの脆弱性
    * https://www.security-next.com/165400

## KEV
* CVE-2024-20767 Adobe ColdFusion Improper Access Control Vulnerability
* CVE-2024-35250 Microsoft Windows Kernel-Mode Driver Untrusted Pointer Dereference Vulnerability
    * https://www.bleepingcomputer.com/news/security/windows-kernel-bug-now-exploited-in-attacks-to-gain-system-privileges/
* CVE-2024-55956 Cleo Multiple Products Unauthenticated File Upload Vulnerability
* CVE-2018-14933 NUUO NVRmini Devices OS Command Injection Vulnerability
* CVE-2022-23227 NUUO NVRmini 2 Devices Missing Authentication Vulnerability
* CVE-2019-11001 Reolink Multiple IP Cameras OS Command Injection Vulnerability
* CVE-2021-40407 Reolink RLC-410W IP Camera OS Command Injection Vulnerability
* CVE-2024-12356 BeyondTrust Privileged Remote Access (PRA) and Remote Support (RS) Command Injection Vulnerability

# その他

* Kali Linux 2024.4 released
    * https://www.bleepingcomputer.com/news/security/kali-linux-20244-released-with-14-new-tools-deprecates-some-features/
* Microsoft 365 アクティベーション ランダムで無効になる不具合
    * https://news.mynavi.jp/techplus/article/20241220-3090506/
    * https://www.theregister.com/2024/12/20/microsoft_office_activation_issue/
