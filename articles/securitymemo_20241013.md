---
title: "2024/10/13 週 セキュリティニュースメモ"
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
    * https://www3.nhk.or.jp/news/html/20241018/k10014613281000.html
* 横須賀市 ライクキッズ株式会社 ランサムウェア被害
    * https://shonanjin.com/news/yokosuka-server-security-issue/
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
    * https://thehackernews.com/2024/10/critical-kubernetes-image-builder.html
* CVE-2024-9634 WP Plugin RCE
    * https://securityonline.info/cve-2024-9634-cvss-9-8-critical-givewp-flaw-exposes-100000-wordpress-sites-to-rce/
* CVE-2024-45844 BIG-IP 権限昇格の脆弱性
    * https://www.securityweek.com/f5-big-ip-updates-patch-high-severity-elevation-of-privilege-vulnerability/
    * https://securityonline.info/f5-big-ip-vulnerability-cve-2024-45844-access-control-bypass-risk-poc-available/
* CVE-2024-38814 VMWare HCX SQLi RCEの脆弱性
    * https://securityonline.info/broadcom-warns-of-high-risk-vmware-hcx-vulnerability-cve-2024-38814/
* CVE-2024-48904 Trend Micro Cloud Edge CommandInjectionの脆弱性
    * https://securityonline.info/cve-2024-48904-cvss-9-8-critical-command-injection-vulnerability-in-trend-micro-cloud-edge/
* CVE-2024-44133 macOS HMSurf ユーザの同意なしにSafariからカメラや位置情報取得ができる脆弱性
    * https://innovatopia.jp/cyber-security/cyber-security-news/43554/
    * https://www.darkreading.com/vulnerabilities-threats/macos-safari-exploit-camera-mic-browser-data
    * https://www.securityweek.com/microsoft-macos-vulnerability-potentially-exploited-in-adware-attacks/
* CVE-2024-9264 Grafana RCE
    * https://securityonline.info/patch-now-grafana-hit-by-9-9-severity-rce-vulnerability-cve-2024-9264/
## KEV
* CVE-2024-40711 Veeam Backup and Replication Deserialization Vulnerability
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
* イギリス大使館 都内の中高一貫校でイギリスのサイバーセキュリティー授業　
    * https://topics.smt.docomo.ne.jp/article/ntv_news24/world/ntv_news24-2024101701474749?fm=latestnews
    * https://news.ntv.co.jp/category/international/987e1ed2844a41559926660a212cc536
* Microsoft 9/2-9/19 の間EntraやSentinel等のログが取得できていなかったバグがあり、顧客へ警告
    * https://www.bleepingcomputer.com/news/security/microsoft-warns-it-lost-some-customers-security-logs-for-a-month/
