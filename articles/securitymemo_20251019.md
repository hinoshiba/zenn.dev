---
title: "2025/10/19 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見たニュースである事に留意ください

# 事件事故

* アスクル ランサムウェア被害。無印良品にも影響
    * https://www.itmedia.co.jp/enterprise/articles/2510/21/news039.html
    * https://www.nikkansports.com/general/news/202510200000835.html
    * https://www.theregister.com/2025/10/21/muji_askul_ransomware/
    * https://www.security-next.com/176018

# 攻撃、脅威

# 脆弱性

* CVE-2025-11702 GitLab Runnner Hijacking
    * https://securityonline.info/gitlab-patches-high-runner-hijacking-flaw-cve-2025-11702-and-multiple-dos-vulnerabilities/
* CVE-2025-20350 Cisco IP-Phone DoS
    * https://securityonline.info/cisco-patches-high-severity-cve-2025-20350-dos-flaw-in-desk-and-ip-phones/
* CVE-2025-59287 WSUS RCE
    * https://securityboulevard.com/2025/10/windows-server-update-service-wsus-remote-code-execution-vulnerability-cve-2025-59287-notice/
    * https://thehackernews.com/2025/10/microsoft-issues-emergency-patch-for.html
    * https://www.bleepingcomputer.com/news/security/hackers-now-exploiting-critical-windows-server-wsus-flaw-in-attacks/
    * https://www.securityweek.com/critical-windows-server-wsus-vulnerability-exploited-in-the-wild/
    * https://www.bleepingcomputer.com/news/security/microsoft-releases-windows-server-emergency-updates-for-critical-wsus-rce-flaw/
* CVE-2025-62168 Critical Squid Proxy HTTP Credentials and Security Tokens がリークする可能性
    * https://securityonline.info/critical-squid-proxy-flaw-cve-2025-62168-cvss-10-0-leaks-http-credentials-and-security-tokens-via-error-handling/
    * https://www.security-next.com/176014


## KEV
* CVE-2025-61932 Motex LANSCOPE Endpoint Manager Improper Verification of Source of a Communication Channel Vulnerability
* CVE-2022-48503 Apple Multiple Products Unspecified Vulnerability 
* CVE-2025-2746 Kentico Xperience Staging Sync Server Digest Password Authentication Bypass Vulnerability
* CVE-2025-2747 Kentico Xperience Staging Sync Server None Password Type Authentication Bypass Vulnerability
* CVE-2025-33073 Microsoft Windows SMB Client Improper Access Control Vulnerability 
* CVE-2025-61884 Oracle E-Business Suite Server-Side Request Forgery (SSRF) Vulnerability
* CVE-2025-54236 Adobe Commerce and Magento Improper Input Validation Vulnerability
* CVE-2025-59287 Microsoft Windows Server Update Service (WSUS) Deserialization of Untrusted Data Vulnerability 


# その他

* Windows 11 localhostのHTTP/2 で接続に関する不具合(修正済み)
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-updates-break-localhost-127001-http-2-connections/
* AWS US-EAST-1 障害
    * https://aws.amazon.com/message/101925/
* 
    * https://www.securityweek.com/microsoft-disables-downloaded-file-previews-to-block-ntlm-hash-leaks/
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-disables-preview-pane-for-downloads-to-block-ntlm-theft-attacks/
