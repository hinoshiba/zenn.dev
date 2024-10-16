---
title: "2024/10/13 週 セキュリティニュースメモ"
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

* ゲームフリーク社、従業員情報等がリーク
    * https://www.darkreading.com/cyberattacks-data-breaches/insider-info-pokemon-allegedly-leaked-gaming-hack
    * https://www.bleepingcomputer.com/news/security/pokemon-dev-game-freak-confirms-breach-after-stolen-data-leaks-online/
* ダークマーケット販売中のCiscoに関するデータ、Ciscoは事実を調査中
    * https://www.theregister.com/2024/10/15/cisco_confirm_ongoing_investigation/
* サイゼリヤ、ランサムウェア被害の可能性
    * https://www.oricon.co.jp/news/2349644/full/
    * https://www.sponichi.co.jp/society/news/2024/10/16/kiji/20241016s00042000296000c.html
    * https://www.hokkaido-np.co.jp/article/1076125/
* 山梨県　県のHP海外からのアクセス負荷により一時閲覧できず
    * https://news.ntv.co.jp/n/ybs/category/society/ys201b2ab7c3f8494982ea006e1cc6713f
# 脆弱性

* CVE-2024-9487 GitHub Enterprise 認証bypass
    * https://securityonline.info/github-enterprise-server-patches-critical-security-flaw-cve-2024-9487-cvss-9-5/
    * https://www.securityweek.com/github-patches-critical-vulnerability-in-enterprise-server/
* CVE-2024-35250 6月に修正されたWindows権限昇格の脆弱性 PoCリリース
    * https://securityonline.info/poc-exploit-release-for-windows-kernel-mode-driver-elevation-of-privilege-flaw-cve-2024-35250/
* CVE-2024-45731 and CVE-2024-45733 Splunk 任意のコード実行の脆弱性
    * https://securityonline.info/splunk-patches-critical-vulnerabilities-including-remote-code-execution-flaws/
* CVE-2024-9486 Kubernetes 上のVMへのRootアクセスの脆弱性。builderアカウントを無効化するワークアラウンドあり
    * https://www.theregister.com/2024/10/16/critical_kubernetes_image_builder_bug/
    * https://www.bleepingcomputer.com/news/security/critical-kubernetes-image-builder-flaw-gives-ssh-root-access-to-vms/
    * https://securityonline.info/cve-2024-9486-cvss-9-8-kubernetes-image-builder-flaw-exposes-vms-to-root-access/
* CVE-2024-9634 WP Plugin RCE
    * https://securityonline.info/cve-2024-9634-cvss-9-8-critical-givewp-flaw-exposes-100000-wordpress-sites-to-rce/

## KEV
* CVE-2024-30088 Microsoft Windows Kernel TOCTOU Race Condition Vulnerability
* CVE-2024-9680 Mozilla Firefox Use-After-Free Vulnerability
* CVE-2024-28987 SolarWinds Web Help Desk Hardcoded Credential Vulnerability

# その他

* Chrome uBlockOriginを含むいくつかの広告ブロッカー拡張機能がもう直ぐブロックされるとのこと。のManifestV2拡張機能仕様非推奨化の一環として。
    * https://www.bleepingcomputer.com/news/google/google-warns-ublock-origin-and-other-extensions-may-be-disabled-soon/
* FIDO、パスキーのクロスプラットフォームに関する提案
    * https://www.bleepingcomputer.com/news/security/new-fido-proposal-lets-you-securely-move-passkeys-across-platforms/
    * https://thehackernews.com/2024/10/fido-alliance-drafts-new-protocol-to.html
* Microsoft アカウントでパスキーが同期されるリリースを予定
    * https://blogs.windows.com/windowsdeveloper/2024/10/08/passkeys-on-windows-authenticate-seamlessly-with-passkey-providers/
* Windows 10 のサポート終了に伴う注意喚起 ipa
    * https://www.ipa.go.jp/security/security-alert/2024/win10_eos.html
