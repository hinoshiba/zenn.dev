---
title: "2024/09/01 週 セキュリティニュースメモ"
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

* ロンドンの交通事業者(TfL)、サイバー攻撃を受けている。サービス影響は、現状ない
    * https://www.bleepingcomputer.com/news/security/transport-for-london-discloses-ongoing-cyber-security-incident/


# 脆弱性
* CVE-2024-8387 Firefox, Thunderbird 任意のコード実行の脆弱性
    * https://www.tenable.com/cve/CVE-2024-8387
* CVE-2024-38811 VMWare Fusion 任意のコード実行の脆弱性
    * https://www.securityweek.com/vmware-patches-high-severity-code-execution-flaw-in-fusion/
    * https://securityonline.info/cve-2024-38811-code-execution-vulnerability-discovered-in-vmware-fusion/
    * https://www.security-next.com/161455
    * https://news.mynavi.jp/techplus/article/20240905-3018694/
* CVE-2024-45195 Apache OFBiz 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/apache-fixes-critical-ofbiz-remote-code-execution-vulnerability/
    * https://www.securityweek.com/apache-makes-another-attempt-at-patching-exploited-rce-in-ofbiz/
    * https://thehackernews.com/2024/09/apache-ofbiz-update-fixes-high-severity.html
* CVE-2024-20439 Cisco ISE 未認証のコード実行
    * https://www.securityweek.com/cisco-patches-critical-vulnerabilities-in-smart-licensing-utility/
* CVE-2024-20469 Cisco ISE ルート権限でのコード実行
    * https://www.bleepingcomputer.com/news/security/cisco-fixes-root-escalation-vulnerability-with-public-exploit-code/
* CVE-2024-32896 Google Pixcel 権限昇格の脆弱性。EoSモデルにもバックポート
    * https://www.bleepingcomputer.com/news/security/google-backports-fix-for-pixel-eop-flaw-to-other-android-devices/
    * https://thehackernews.com/2024/09/google-confirms-cve-2024-32896.html
    * https://www.securityweek.com/androids-september-2024-update-patches-exploited-vulnerability/
    * https://securityonline.info/google-patches-actively-exploited-zero-day-in-september-android-update/
* CVE-2024-7720 HP Security Manager 任意のコード実行の脆弱性
    * https://www.security-next.com/161471
* CVE-2024-45076 IBM webMethods Integration 認証済みユーザによる任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-45076-cvss-9-9-critical-flaw-in-ibm-webmethods-integration-demand-immediate-action/
* CVE-2024-7923 RedHat コンテンツ配備システム Pulpcore に未認証の管理者アクセスの脆弱性
    * https://securityonline.info/red-hat-issues-critical-patch-for-pulpcore-authentication-bypass-flaw-cve-2024-7923/
* CVE-2024-7012 Red Hat Satellite 未認証のアクセスの脆弱性
    * https://securityonline.info/cve-2024-7012-cvss-9-8-critical-foreman-flaw-exposes-red-hat-satellite-to-unauthorized-access/
* CVE-2024-44000 WordPress Plugin LiteSpeedCache 管理者権限窃取の可能性
    * https://thehackernews.com/2024/09/critical-security-flaw-found-in.html
    * https://www.securityweek.com/litespeed-cache-plugin-vulnerability-exposes-millions-of-wordpress-sites-to-attacks/
* CVE-2024-26581 Linuxへのルート侵害の脆弱性
    * https://securityonline.info/cve-2024-26581-poc-exploit-released-linux-systems-at-risk-of-root-compromise/
* CVE-2024-7591 Progress LoadMaster 未認証のコード実行の脆弱性
    * https://securityonline.info/cve-2024-7591-cvss-10-critical-vulnerability-discovered-in-progress-loadmaster/
    * https://thehackernews.com/2024/09/progress-software-issues-patch-for.html
    * https://www.bleepingcomputer.com/news/security/progress-loadmaster-vulnerable-to-10-10-severity-rce-flaw/
* KEV
    * CVE-2021-20123 Draytek VigorConnect Path Traversal Vulnerability
    * CVE-2021-20124 Draytek VigorConnect Path Traversal Vulnerability
    * CVE-2024-7262 Kingsoft WPS Office Path Traversal Vulnerability


# その他

* Docker OSX プロジェクト、DMCA削除要請により、削除
    * https://www.bleepingcomputer.com/news/security/docker-osx-image-used-for-security-research-hit-by-apple-dmca-takedown/
* ブラジル当局、連邦最高裁判所の命令に従いXへの通信遮断
    * https://jp.reuters.com/economy/industry/CGYR7S4IQBJMRNFDFZL3HKYINM-2024-09-01/
* Linux Kernel 6.12 にて、カーネルパニック等でのエラーメッセージをQRコードにする機能が追加
    * https://securityonline.info/qr-codes-coming-to-linux-kernel-panics-with-6-12-release/
* IBM QRader PaloAltoに買収
    * https://www.theregister.com/2024/09/04/palo_alto_networks_ibm_qradar/
* Ciscoのオンラインストアに悪意のあるJSが注入されクレジットカード情報や認証情報が盗まれていた
    * https://www.bleepingcomputer.com/news/security/hackers-inject-malicious-js-in-cisco-store-to-steal-credit-cards-credentials/
    * https://news.mynavi.jp/techplus/article/20240906-3019238/
* Yubikeyに複製の脆弱性。ただしコストは$11,000
    * https://securityboulevard.com/2024/09/fwbifx/
    * https://arstechnica.com/security/2024/09/yubikeys-are-vulnerable-to-cloning-attacks-thanks-to-newly-discovered-side-channel/
