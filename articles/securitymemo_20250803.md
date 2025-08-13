---
title: "2025/08/03 週 セキュリティニュースメモ"
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
* 法政大、1万6000人超の情報漏えいか　不正アクセスで
    * https://ascii.jp/elem/000/004/311/4311737/
* Air France KLM 航空 顧客ポータルから顧客情報が盗まれた。パスポート等の情報は流出していないと広報
    * https://www.darkreading.com/cyberattacks-data-breaches/air-france-klm-data-breach
    * https://www.securityweek.com/air-france-klm-say-hackers-accessed-customer-data/

# 攻撃、脅威

* Perplexity AI robots.txt の無視に関して
    * https://securityonline.info/cloudflare-accuses-perplexity-ai-of-evading-blocks-and-impersonating-chrome-to-scrape-websites/
    * https://blog.cloudflare.com/perplexity-is-using-stealth-undeclared-crawlers-to-evade-website-no-crawl-directives/
    * https://news.mynavi.jp/techplus/article/20250806-3398753/



# 脆弱性

* CVE-2025-54574 Squid RCE
    * https://securityonline.info/critical-squid-vulnerability-cve-2025-54574-allows-remote-code-execution-data-leakage/
* CVE-2025-54254 Adobe AEM Forms XXE の脆弱性
    * https://www.bleepingcomputer.com/news/security/adobe-issues-emergency-fixes-for-aem-forms-zero-days-after-pocs-released/
* Proton Authenticator TOTP Secrets がログで漏れてしまう可能性
    * https://securityonline.info/ios-update-proton-authenticator-bug-leaked-totp-secrets-in-plaintext-logs/
* CVE-2025-24311, CVE-2025-25050, CVE-2025-25215, CVE-2025-24922, CVE-2025-24919 ReVault 攻撃と名付けられたDell管理ソフトウェアに関するWindowsログイン認証bypassの脆弱性
    * https://www.bleepingcomputer.com/news/security/revault-flaws-let-hackers-bypass-windows-login-on-dell-laptops/
    * https://www.securityweek.com/flaws-expose-100-dell-laptop-models-to-implants-windows-login-bypass/

# その他

* ISC2 がAIに関するセキュリティの資格を公開
    * https://www.darkreading.com/cybersecurity-careers/isc2-launches-security-certificate-ai-expertise
    * https://www.isc2.org/Insights/2025/07/ISC2-Launches-AI-Certificate
* Windows 11 SE のサポートを2026 11 月末を予定。Microsoft
    * https://www.theregister.com/2025/08/01/microsoft_abandons_windows_11_se/
* ブロックされたコンテンツへのMicrosoft 外部向けworkbook linkをデフォルトで無効化する 2026/07までにかけて。
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-disable-external-workbook-links-to-blocked-file-types/
* Microsoft AIによるマルウェア分類のプロジェクトProject Ire を開始
    * https://thehackernews.com/2025/08/microsoft-launches-project-ire-to.html
