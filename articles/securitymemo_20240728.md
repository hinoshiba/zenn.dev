---
title: "2024/07/28 週 セキュリティニュースメモ"
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

* DigiCert、ドメインコントロール検証（DCV）プロセスの不備により、数千のSSL/TLS証明書を緊急に取り消し。影響は、全検証の約0.4%であるものの、対象者は、24時間以内に証明書の再発行が必要
    * https://www.cisa.gov/news-events/alerts/2024/07/30/digicert-certificate-revocations
    * https://www.digicert.com/support/certificate-revocation-incident
    * https://securityonline.info/digicert-forced-to-revoke-thousands-of-certificates-due-to-domain-validation-error/
    * https://gbhackers.com/digicert-to-revoke-thousands/
    * https://www.bleepingcomputer.com/news/security/digicert-to-delay-cert-revocations-for-critical-infrastructure/
    * https://thehackernews.com/2024/07/digicert-to-revoke-83000-ssl.html
    * https://www.theregister.com/2024/07/31/digicert_certificates_revoked/
    * https://securityonline.info/digicert-revokes-certificates-what-you-need-to-know/
* Data Breaches for the Month July 2024
    * https://securityboulevard.com/2024/07/data-breaches-for-the-month-july-2024/


# 攻撃、脅威
* Google WorkSpaceの認証機能を用い第三者のアカウントを奪い取る不具合を修正。悪用試みがあり
    * https://securityonline.info/google-patches-workspace-authentication-flaw-thwarting-account-takeover-attempts/
* シャープ、公式EC「COCORO STORE｣で不正アクセス　203件の個人情報流出
    * https://www.watch.impress.co.jp/docs/news/1612161.html
    * https://news.google.com/rss/articles/CBMiKmh0dHBzOi8vc3AubS5qaWppLmNvbS9hcnRpY2xlL3Nob3cvMzI5ODAwOdIBAA?oc=5&hl=en-US&gl=US&ceid=US:en
* たまの湯LINE会員システム 不正アクセスにより6千+4千件の個人情報漏洩の可能性
    * https://cybersecurity-jp.com/news/98484
    * https://www.security-next.com/160307
* ランサムウェアによりOneBlood Blood Bankの業務が一部遅延
    * https://www.securityweek.com/ransomware-attack-hits-oneblood-blood-bank-disrupts-medical-operations/
* Proofpointのプラットフォームが悪用されフィッシングメールが送付される
    * https://securityboulevard.com/2024/07/proofpoint-platform-exploited-to-send-millions-of-spoofed-phishing-emails/
    * https://thehackernews.com/2024/07/proofpoint-email-routing-flaw-exploited.html
* ダークウェブにて、3TBのBausch Health社の医療データ(DEA番号を含む) が販売。Snowflakeとの関係を示唆
    * https://dailydarkweb.net/threat-actor-claims-to-sell-bausch-health-data-including-1-6-million-dea-numbers/

# 脆弱性

* CVE-2024-5285 WP Affiliate Platform 情報削除 CSRF
    * https://wpscan.com/vulnerability/792f3904-88bd-47d1-9049-afccdd74853a/
* OAuthの実装不備によるXSSの脆弱性。HotJar and Business Insider を例にSalt Labsが報告
    * https://www.securityweek.com/millions-of-websites-susceptible-xss-attack-via-oauth-implementation-flaw/
    * https://salt.security/blog/over-1-million-websites-are-at-risk-of-sensitive-information-leakage---xss-is-dead-long-live-xss
    * https://www.darkreading.com/endpoint-security/oauth-xss-attack-millions-web-users-account-takeover
* CVE-2024-42225 linux kernel 未初期化のリソース使用
    * https://cvefeed.io/vuln/detail/CVE-2024-42225
* CVE-2024-37085 6月末に公開された ESXi 認証bypassの脆弱性がランサムウェア攻撃に用いられている注意喚起
    * https://www.bleepingcomputer.com/news/security/cisa-warns-of-vmware-esxi-bug-exploited-in-ransomware-attacks/
    * https://www.darkreading.com/cloud-security/ransomware-gangs-exploit-esxi-bug-for-instant-mass-encryption-of-vms
    * https://securityonline.info/cve-2024-37085-vmware-esxi-vulnerability-exploited-by-ransomware-gangs/
    * https://www.security-next.com/160345
* Appleデバイスセキュリティパッチ更新
    * https://www.cisa.gov/news-events/alerts/2024/07/30/apple-releases-security-updates-multiple-products
    * https://www.securityweek.com/apple-rolls-out-security-updates-for-ios-macos/
    * https://www.security-next.com/160322
    * https://www.security-next.com/160310
    * CVE-2024-23296  bypass kernel memory protections
        * https://www.bitdefender.com/blog/hotforsecurity/apple-patches-rtkit-flaw-presumably-exploited-by-hackers-on-macs/
        * https://securityonline.info/apple-extends-zero-day-patch-to-older-macs-urges-immediate-update/
    * CVE-2024-6387 regreSSHion
        * https://securityonline.info/critical-openssh-vulnerability-regresshion-threatens-macos-users/
    * ロック状態のiPhoneから連絡先等の情報をSiri経由で確認できる脆弱性
        * https://www.darkreading.com/vulnerabilities-threats/siri-bug-enables-data-theft-on-locked-apple-devices
* CVE-2024-41924 EC-CUBE4 第三者に管理者権限で任意のパッケージをインストールされる可能性
    * https://nvd.nist.gov/vuln/detail/CVE-2024-41924
* CVE-2024-6576 Progress MOVEit Transfer 権限昇格の脆弱性
    * https://securityonline.info/progress-software-issues-security-alert-for-moveit-transfer-users-cve-2024-6576/
    * https://www.security-next.com/160340
* CVE-2024-5807 WordPress Plugin Bussiness Card, 悪意のあるPHPがアップロードされる可能性
    * https://vulners.com/nvd/NVD:CVE-2024-5807
* CVE-2024-6412 WordPress Plugin HTML Forms CSRF
    * https://cvefeed.io/vuln/detail/CVE-2024-6412
* CVE-2024-6990 Google Chrome グループポリシー管理Dawnへの初期化不備
    * https://www.security-next.com/160335
    * https://www.bitdefender.com/blog/hotforsecurity/update-browser-google-critical-security-chrome-127-desktop-android/
    * https://securityonline.info/urgent-chrome-update-google-patches-critical-security-flaw-cve-2024-6990/
* CVE-2024-41947 XMLWiki XSS
    * https://jira.xwiki.org/browse/XWIKI-21626
* CVE-2024-7208 CVE-2024-7209 複数のSMTPサーバ、認証されたユーザがその他ユーザになりすますことができる脆弱性
    * https://kb.cert.org/vuls/id/244112
    * https://www.securityweek.com/vulnerabilities-enable-attackers-to-spoof-emails-from-20-million-domains/
    * https://securityonline.info/critical-vulnerability-in-hosted-email-services-exposes-users-to-spoofing-attacks/
* CVE-2024-36401 GeoServer RCE
    * https://securityonline.info/critical-geoserver-rce-flaw-cve-2024-36401-actively-exploited-6284-instances-vulnerable/
* CVE-2024-6698 WordPressPlugin FundEngine 権限昇格の脆弱性
    * https://securityvulnerability.io/vulnerability/CVE-2024-6698
* CVE-2024-41667: OpenAM 任意のコード実行の可能性
    * https://securityonline.info/cve-2024-41667-openam-vulnerability-exposes-authentication-systems-to-critical-risk/
* KEV
    * CVE-2024-4879 ServiceNow Improper Input Validation Vulnerability
    * CVE-2024-5217 ServiceNow Incomplete List of Disallowed Inputs Vulnerability
    * CVE-2023-45249 Acronis Cyber Infrastructure (ACI) Insecure Default Password Vulnerability
    * CVE-2024-37085 VMware ESXi Authentication Bypass Vulnerability

# その他

* Windows11 タスクバーから、タスクの終了が選べるように。デフォルトだと無効
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-taskbar-has-a-hidden-end-task-feature-how-to-turn-it-on/
* X(Twitter) LLMsのトレーニングを開始。オプトアウト手順あり
    * https://www.bleepingcomputer.com/news/security/x-begins-training-grok-ai-with-your-posts-heres-how-to-disable/
    * https://securityonline.info/x-formerly-twitter-silently-trains-ai-on-user-data-sparks-privacy-concerns/
* iOS 18.1 ベータ 公開によりAppleIntelligenceのテスト利用が可能
    * https://www.bleepingcomputer.com/news/apple/apple-ios-181-beta-previews-apple-intelligence-for-the-first-time/
    * https://www.theregister.com/2024/07/30/apple_intelligence_ai_beta/
* 投資ファンド・日本サイバーセキュリティファンド（NCSF）は7月29日、新たに出資者として参加するセキュリティ企業13社を発表
    * https://www.itmedia.co.jp/news/articles/2407/29/news150.html
* PKfail。UEFIセキュアブートのプラットフォームキーがGitHub上に上がっていた。暗号化されていたが４文字パスワードだった
    * https://www.theregister.com/2024/07/29/infosec_roundup/
    * https://www.binarly.io/blog/pkfail-untrusted-platform-keys-undermine-secure-boot-on-uefi-ecosystem
    * https://gigazine.net/news/20240726-pkfail/
    * https://news.mynavi.jp/techplus/article/20240730-2993248/
* AzureやM365にて複数のサービスが8時間以上不具合。DDoSを防御する機構自体に不具合があり攻撃が増大した
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-365-and-azure-outage-takes-down-multiple-services/
    * https://securityboulevard.com/2024/07/microsoft-ddos-attack-on-azure-services-exacerbated-by-defense-error/
    * https://www.darkreading.com/cloud-security/microsoft-azure-ddos-attack-amplified-cyber-defense-error
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-says-massive-azure-outage-was-caused-by-ddos-attack/
    * https://www.theregister.com/2024/07/31/microsoft_ddos_azure/
    * https://securityboulevard.com/2024/07/breaking-news-microsoft-azure-faces-service-disruption-amidst-ddos-attack/
* Skype 広告フリーに。
    * https://www.theregister.com/2024/07/31/skype_adfree/
* IPA 情報セキュリティ白書2024
    * https://www.ipa.go.jp/publish/wp-security/2024.html
* TryCloudflareというWebサービス確認サービスを用い、マルウェア等を配布する手口
    * https://www.bleepingcomputer.com/news/security/hackers-abuse-free-trycloudflare-to-deliver-remote-access-malware/
* UK当局、Russian ComsのTakeDown
    * https://www.bleepingcomputer.com/news/security/uk-takes-down-russian-comms-caller-id-spoofing-platform-used-to-scam-170-000-people/
* Microsoft 365 Personal and Family にて、無料のDefenderVPNを提供開始。月50GiBまで。
    * https://securityonline.info/microsoft-365-boosts-security-with-free-defender-vpn/
* ICI リスクアセスメントツール公開
    * https://blog.itochuci.co.jp/entry/2024/07/31/160000
