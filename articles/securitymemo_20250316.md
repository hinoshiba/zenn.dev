---
title: "2025/03/17 週 セキュリティニュースメモ"
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

# 脆弱性

* CVE-2025-27407 GraphQL-Ruby RCE
    * https://securityonline.info/cve-2025-27407-cvss-9-1-critical-graphql-ruby-flaw-exposes-millions-to-rce/
* CVE-2025-30066 GitHub Actions tj-actions/changed-files への悪意のあるコード注入
    * https://securityonline.info/popular-github-action-tj-actions-changed-files-compromised-cve-2025-30066/
    * https://www.bleepingcomputer.com/news/security/supply-chain-attack-on-popular-github-action-exposes-ci-cd-secrets/
    * https://www.theregister.com/2025/03/17/supply_chain_attack_github/
    * https://thehackernews.com/2025/03/github-action-compromise-puts-cicd.html
    * https://www.securityweek.com/popular-github-action-targeted-in-supply-chain-attack/
    * 依存先の、`reviewdog/action-setup` によるものとのブログをwizが公開
        * https://www.wiz.io/blog/new-github-action-supply-chain-attack-reviewdog-action-setup
* CVE-2025-26909 WordPress Plugin GHOST RCE
    * https://www.bleepingcomputer.com/news/security/wordpress-security-plugin-wp-ghost-vulnerable-to-remote-code-execution-bug/
* CVE-2025-24071 今月のWindowsUpdateで修正されたNTMLハッシュを細工された圧縮ファイルで盗む脆弱性、PoCリリース
    * https://securityonline.info/poc-released-windows-explorer-cve-2025-24071-vulnerability-exposes-ntlm-hashes/
* CVE-2024-11131 Synology Camera 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-11131-cvss-9-8-critical-vulnerability-found-in-synology-camera-firmware/
* CVE-2025-0755 MongoDB ドライバ不備によりバッファオーバーフローの脆弱性
    * https://securityonline.info/cve-2025-0755-mongodb-c-driver-vulnerability-could-lead-to-buffer-overflow/
*  CVE-2024-10441 Synology 任意のコード実行の脆弱性。Synology BeeStation Manager (BSM), Synology DiskStation Manager (DSM), and Synology Unified Controller (DSMUC) など。
    * https://securityonline.info/cve-2024-10441-cvss-9-8-synology-patches-critical-code-execution-flaw-in-multiple-products/
* ZDI-CAN-25373 Windows lnk によるコード実行の脆弱性。
    * https://www.bleepingcomputer.com/news/security/new-windows-zero-day-exploited-by-11-state-hacking-groups-since-2017/
* CVE-2025-1861 PHP stream HTTP wrapperのバッファ不足によりDoSの可能性
    * https://securityonline.info/multiple-security-vulnerabilities-plague-php-exposing-applications-to-risk/
* CVE-2024-540385 HPE Cray XD670 管理者による未認証のアクセスの脆弱性
    * https://securityonline.info/hpe-cray-vulnerability-cve-2024-540385-authentication-bypass-threat-cvss-10-alert/


## KEV
* CVE-2025-1316 Edimax IC-7100 IP Camera OS Command Injection Vulnerability
* CVE-2024-48248 NAKIVO Backup and Replication Absolute Path Traversal Vulnerability
* CVE-2017-12637 SAP NetWeaver Directory Traversal Vulnerability


# その他

* Wiz GoogleにJoin
    * https://www.wiz.io/blog/wiz-joining-google
* Ubuntu 25.10 では、coreutilsをRUSTに置き換えることが検討されている
    * https://www.theregister.com/2025/03/19/ubuntu_2510_rust/
