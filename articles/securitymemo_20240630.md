---
title: "2024/06/30 週 セキュリティニュースメモ"
emoji: "🔖"
type: "tech"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
* あくまで、発見した週に記入します
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

* UberやX, TikTok等で利用する本人 確認サービス AU10TIX データ漏洩の可能性。(AU10TIXとして、悪用確認は、無しとのこと)
    * https://news.mynavi.jp/techplus/article/20240629-2975378/
    * https://www.malwarebytes.com/blog/news/2024/06/driving-licences-and-other-official-documents-leaked-by-authentication-service-used-by-uber-tiktok-x-and-more

# 攻撃、脅威

* クボタクレジット ランサムウェア
    * https://www.itmedia.co.jp/news/articles/2407/01/news155.html

# 脆弱性
* CVE-2024-2386 WP MAPS for WordPress SQL Injectionの脆弱性
    * https://securityvulnerability.io/vulnerability/CVE-2024-2386
* CVE-2024-5535 OpenSSL 一部API関数にDoSの脆弱性。悪用は、攻撃者の制御下に限定的
    * https://www.security-next.com/159094
    * https://www.openssl.org/news/secadv/20240627.txt
* CVE-2024-6387 OpenSSH 未認証の上位権限でのRCE
    * https://securityboulevard.com/2024/07/a-playbook-for-detecting-the-openssh-vulnerability-cve-2024-6387-regresshion/
    * https://www.darkreading.com/cloud-security/regresshion-bug-threatens-takeover-of-millions-of-linux-systems
    * https://www.theregister.com/2024/07/01/regresshion_openssh/
    * https://www.bleepingcomputer.com/news/security/new-regresshion-openssh-rce-bug-gives-root-on-linux-servers/
    * https://www.securityweek.com/millions-of-openssh-servers-potentially-vulnerable-to-remote-regresshion-attack/
    * https://thehackernews.com/2024/07/new-openssh-vulnerability-could-lead-to.html
    * https://securityonline.info/cve-2024-6387-critical-openssh-unauthenticated-rce-flaw-regresshion-exposes-millions-of-linux-systems/
* CVE-2024-38513 Fiber セッショントークンのインジェクション脆弱性
    * https://github.com/gofiber/fiber/security/advisories/GHSA-98j2-3j3p-fw2v
    * https://nvd.nist.gov/vuln/detail/CVE-2024-38513
* CVE-2024-31320 アプリがsetSkipPromptでプロンプトをスキップできるセキュリティ問題を修正
    * https://source.android.com/docs/security/bulletin/2024-07-01
* CVE-2024-20399 Cisco NX-OS 管理者権限での任意のコード実行に関する脆弱性
    * https://www.bleepingcomputer.com/news/security/cisco-warns-of-nx-os-zero-day-exploited-to-deploy-custom-malware/
    * https://securityonline.info/cve-2024-20399-cisco-nx-os-zero-day-vulnerability-under-active-attack/
* CVE-2024-0193 1月に公開されたLinuxの権限昇格脆弱性 PoCリリース
    * https://securityonline.info/poc-exploit-published-for-linux-kernel-privilege-escalation-flaw-cve-2024-0193/
* CVE-2024-5261 LibreOffice データ傍受や操作を行われる可能性
    * https://securityonline.info/cve-2024-5261-cvss-10-libreoffice-patches-critical-vulnerability-in-libreofficekit/
    * https://www.security-next.com/159105
# その他
* Windows11 再起動ループ不具合改善版のWindowsUpdate配信開始
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-resumes-rollout-of-windows-11-kb5039302-update-for-most-users/
* Microsoft クラウドサービスに関してもCVE番号を付与していくと発表
    * https://securityonline.info/microsoft-issues-cve-numbers-for-cloud-service-vulnerabilities/
* CocoaPodsの脆弱性によりAppleデバイスサプライチェーンアタックの危機
    * https://thehackernews.com/2024/07/critical-flaws-in-cocoapods-expose-ios.html
    * https://www.darkreading.com/cloud-security/apple-cocoapods-bugs-expose-apps-code-injection
    * v
