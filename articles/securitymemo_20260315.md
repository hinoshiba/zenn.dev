---
title: "2026/03/15 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。

# 事件事故

* Starbucks 従業員ポータルをもしたフィッシングにより従業員情報が流出の可能性
    * https://www.bleepingcomputer.com/news/security/starbucks-discloses-data-breach-affecting-hundreds-of-employees/

# 攻撃、脅威

* GlassWorm
    * https://qiita.com/sarubot/items/df077776b293163e0a42
* Trivy サプライチェーン攻撃により侵害される
    * https://gbhackers.com/trivy-vulnerability-scanner-compromised/
    * https://gbhackers.com/microsoft-to-detect-defend-against-trivy-supply-chain-attack/
    * https://gbhackers.com/aqua-securitys-trivy-scanner-hit-by-supply-chain-attack/
    * https://gbhackers.com/trivy-supply-chain/
    * https://www.security-next.com/182637

# 脆弱性
* CVE-2026-32746 Telnetd RCE脆弱性
    * https://www.security-next.com/182181
    * https://gbhackers.com/critical-telnetd-vulnerability/
    * https://thehackernews.com/2026/03/critical-telnetd-flaw-cve-2026-32746.html
* CVE-2026-20643 Apple WebKit セキュリティ機能の迂回
    * https://gbhackers.com/apple-webkit-security-flaw/
    * https://www.securityweek.com/apple-debuts-background-security-improvements-with-fresh-webkit-patches/
* CVE-2026-3888 Ubuntu 権限昇格の脆弱性
    * https://gbhackers.com/ubuntu-desktop-vulnerability/
* CVE-2026-21643 FortiClient Enterprise Management SQLi
    * https://gbhackers.com/forticlient-hit-by-severe-sql-injection-vulnerability/
* CVE-2026-26954 SandBox JS RCE
    * https://securityonline.info/golden-ticket-critical-10-cvss-sandboxjs-flaw-cve-2026-26954-rce/
* CVE-2026-33001 Jenkins RCE
    * https://securityonline.info/pipeline-poison-critical-jenkins-vulnerabilities-rce-cve-2026-33001/


## KEV
* CVE-2026-20963 Microsoft SharePoint Deserialization of Untrusted Data Vulnerability
* CVE-2025-66376 Synacor Zimbra Collaboration Suite (ZCS) Cross-Site Scripting Vulnerability
* CVE-2025-47813 Wing FTP Server Information Disclosure Vulnerability

# その他
* 「セキュリティ10大脅威2026 」組織編の解説書を公開 - IPA
    * https://www.security-next.com/182229
