---
title: "2025/09/21 週 セキュリティニュースメモ"
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

* Steamにて「マルウェア入り無料ゲーム」により総額約2200万円規模の被害発生との報道。被害に遭う瞬間が生配信される異例の事態に
    * https://automaton-media.com/articles/newsjp/blockblasters-20250923-358730/
    * https://www.bleepingcomputer.com/news/security/verified-steam-game-steals-streamers-cancer-treatment-donations/
* イギリスやベルギーなど空港でシステム障害 サイバー攻撃か
    * https://www3.nhk.or.jp/news/html/20250921/k10014928781000.html
    * https://topics.smt.docomo.ne.jp/article/ntv_news24/world/ntv_news24-2025092005533361

# 攻撃、脅威

* Rust パッケージ、暗号資産を狙うパッケージ改ざん
    * https://www.bleepingcomputer.com/news/security/malicious-rust-packages-on-cratesio-steal-crypto-wallet-keys/
    * https://socket.dev/blog/two-malicious-rust-crates-impersonate-popular-logger-to-steal-wallet-keys
* SalesForce AI系支援による情報流出ForcedLeak の改善
    * https://thehackernews.com/2025/09/salesforce-patches-critical-forcedleak.html
* GitHubの通知を悪用しフィッシング
    * https://www.bleepingcomputer.com/news/security/github-notifications-abused-to-impersonate-y-combinator-for-crypto-theft/
* GitHub NPMパッケージのサプライチェーンアタックに対するセキュリティ強化
    * https://www.securityweek.com/github-boosting-security-in-response-to-npm-supply-chain-attacks/
    * https://www.darkreading.com/application-security/github-secure-supply-chain-npm-hacks-ramp-up
    * https://www.theregister.com/2025/09/23/github_npm_registry_security/
* Cloudflare 22.2Tbps のDDoSを低減
    * https://www.bleepingcomputer.com/news/security/cloudflare-mitigates-new-record-breaking-222-tbps-ddos-attack/
* Microsoft Teamのインストーラを語るマルバタイジング
    * https://www.bleepingcomputer.com/news/security/fake-microsoft-teams-installers-push-oyster-malware-via-malvertising/

# 脆弱性

* CVE-2025-20333 Cisco ASA RCE
    * https://www.bleepingcomputer.com/news/security/cisco-warns-of-asa-firewall-zero-days-exploited-in-attacks/
* CVE-2025-20352 Cisco SNMP 脆弱性によるRootアクセス
    * https://securityonline.info/cisco-snmp-flaw-cve-2025-20352-actively-exploited-patch-now-to-stop-root-access/
    * https://www.bleepingcomputer.com/news/security/cisco-warns-of-ios-zero-day-vulnerability-exploited-in-attacks/
* Microsoft Microsoft Entra ID に欠陥があり、テナントに不正にアクセスを行われた可能性がある
    * https://www.bleepingcomputer.com/news/security/microsoft-entra-id-flaw-allowed-hijacking-any-companys-tenant/


# その他
* Kali 2025.3 リリース
    * https://www.bleepingcomputer.com/news/security/kali-linux-20253-released-with-10-new-tools-wifi-enhancements/
