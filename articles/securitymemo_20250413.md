---
title: "2025/04/13 週 セキュリティニュースメモ"
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
* IIJメールサービス設備内に不正プログラム - 最大6493契約で情報漏洩のおそれ
    * https://www.security-next.com/169332
    * https://www.security-next.com/169596
    * https://www.ipa.go.jp/security/security-alert/2025/20250418-jvn.html
    * https://www.security-next.com/169498

# 攻撃、脅威

# 脆弱性

* CVE-2025-32754 Jenkins ssh-agentのDockerImage、同一のSSHホストキーを利用するため、他エージェントへの接続が可能な脆弱性
    * https://securityonline.info/jenkins-docker-images-vulnerable-to-ssh-host-key-reuse/
* CVE-2025-3619 Google Chrome Heap overflow の脆弱性
    * https://securityonline.info/critical-chrome-security-update-patch-cve-2025-3619-cve-2025-3620-now/
* CVE-2025-32102 CrushFTP SSRF
    * https://securityonline.info/crushftp-hit-by-ssrf-and-directory-traversal-vulnerabilities-cve-2025-32102-cve-2025-32103/
* CVE-2025-3509 GHE 任意のコード実行の脆弱性
    * https://securityonline.info/github-enterprise-server-vulnerabilities-expose-risk-of-code-execution-and-data-leaks/

## KEV
* CVE-2025-31200 Apple Multiple Products Memory Corruption Vulnerability
    * https://www.securityweek.com/apple-pushes-ios-macos-patches-to-quash-two-zero-days/
    * https://thehackernews.com/2025/04/apple-patches-two-actively-exploited.html
    * https://www.bleepingcomputer.com/news/security/apple-fixes-two-zero-days-exploited-in-targeted-iphone-attacks/
* CVE-2025-31201 Apple Multiple Products Arbitrary Read and Write Vulnerability
    * https://www.securityweek.com/apple-pushes-ios-macos-patches-to-quash-two-zero-days/
    * https://thehackernews.com/2025/04/apple-patches-two-actively-exploited.html
    * https://www.bleepingcomputer.com/news/security/apple-fixes-two-zero-days-exploited-in-targeted-iphone-attacks/
* CVE-2025-24054 Microsoft Windows NTLM Hash Disclosure Spoofing Vulnerability

# その他

* MITRE への米国政府資金援助が、4/16に終了予定
    * https://thehackernews.com/2025/04/us-govt-funding-for-mitres-cve-ends.html
    * https://www.bleepingcomputer.com/news/security/mitre-warns-that-funding-for-critical-cve-program-expires-today/
    * https://securityonline.info/mitre-warns-of-cve-program-disruption-as-u-s-contract-set-to-expire/
* IPA セキュリティインシデント対応机上演習教材 を公開
    * https://www.ipa.go.jp/security/sec-tools/ttx.html
* JVN CVSS v4 4/21より採用
    * https://jvn.jp/en/nav/info2025041472.html
    * https://news.yahoo.co.jp/articles/241ad414f3e952fc77b48d1038bb2410c97e03d1
