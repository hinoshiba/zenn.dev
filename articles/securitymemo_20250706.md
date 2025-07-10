---
title: "2025/07/06 週 セキュリティニュースメモ"
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

* 多くのeSIM携帯電話にて、eSIMがsimが盗まれる可能性の研究結果 Security Explorations
    * https://www.darkreading.com/endpoint-security/esim-bug-millions-phones-spying-takeover
    * https://www.securityweek.com/esim-hack-allows-for-cloning-spying/


# 脆弱性

* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-jul
        * https://krebsonsecurity.com/2025/07/microsoft-patch-tuesday-july-2025-edition/
        * https://msrc.microsoft.com/blog/2025/07/202507-security-update/
        * https://www.darkreading.com/application-security/microsoft-patches-137-cves-no-zero-days
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-july-2025-patch-tuesday-fixes-one-zero-day-137-flaws/
* Lenovo `c:\windows\mfgstat.zip` というファイルのADSでコード実行の可能性
    * https://gbhackers.com/writable-file-in-lenovo-path-attackers-evade-applocker/#google_vignette
* CVE-2025-48384 Git submoduleの値にCRが入っている場合にコード実行の可能性
    * https://securityonline.info/git-project-patches-3-flaws-rce-arbitrary-file-writes-buffer-overflow/
* CVE-2025-49533 Adobe製品 コード実行の可能性
    * https://www.securityweek.com/adobe-patches-critical-code-execution-bugs/
* CVE-2025-48367 Redis DoS
    * https://securityonline.info/redis-dos-flaw-cve-2025-48367-authenticated-clients-can-disrupt-service/
    * https://securityonline.info/redis-vulnerability-opens-door-to-remote-code-execution-poc-releases/
* CVE-2025-6948 GitLab XSS
    * https://securityonline.info/gitlab-releases-security-updates-xss-and-authorization-bypass-flaws-patched/

## KEV
* CVE-2014-3931 Multi-Router Looking Glass (MRLG) Buffer Overflow Vulnerability
* CVE-2016-10033 PHPMailer Command Injection Vulnerability
* CVE-2019-5418 Rails Ruby on Rails Path Traversal Vulnerability
* CVE-2019-9621 Synacor Zimbra Collaboration Suite (ZCS) Server-Side Request Forgery (SSRF) Vulnerability
* CVE-2025-5777 Citrix NetScaler ADC and Gateway Out-of-Bounds Read Vulnerability

# その他

