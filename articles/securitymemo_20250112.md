---
title: "2025/01/12 週 セキュリティニュースメモ"
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

* Microsoft MFAに関して障害
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-mfa-outage-blocking-access-to-microsoft-365-apps/


# 攻撃、脅威

* iPhoneユーザに対して、iMessageのフィッシング保護機能を無効化するような誘導するキャンペーン
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/iphone-users-tricked-into-disabling-apple-imessages-phishing-protection

# 脆弱性

* CVE-2025-22777 GiveWP 未認証のPHPオブジェクトインジェクションの脆弱性
    * https://securityonline.info/cve-2025-22777-cvss-9-8-critical-security-alert-for-givewp-plugin-with-100000-active-installations/
* CVE-2024-12847 NETGEAR ルータ 未認証のコマンド実行の脆弱性。PoCあり
    * https://securityonline.info/cve-2024-12847-cvss-9-8-netgear-router-flaw-exploited-in-the-wild-for-years-poc-published/
* CVE-2024-12426 LibreOffice 環境変数等の流出の可能性
    * https://forest.watch.impress.co.jp/docs/news/1653446.html
* CVE-2024-44243 昨年12月に公表されたmacOSのセキュリティ機能bypassの脆弱性、詳細レポートをMicrosoftがリリース
    * https://www.microsoft.com/en-us/security/blog/2025/01/13/analyzing-cve-2024-44243-a-macos-system-integrity-protection-bypass-through-kernel-extensions/
* CVE-2024-54498 昨年12月に公表されたmacOSのsandbox bypassの脆弱性、PoCリリース
    * https://securityonline.info/new-macos-exploit-revealed-poc-for-cve-2024-54498-breaks-sandbox-security/
* CVE-2025-21598 JunOS 細工されたBGPパケットによるDoS
    * https://www.securityweek.com/juniper-networks-fixes-high-severity-vulnerabilities-in-junos-os/

# その他

* 2月のWindowsUpdateにて、Windows10にOutlookがインストールされるとのこと
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-to-force-install-new-outlook-on-windows-10-pcs-in-february/
* LDAPNightmare に関する偽のPoCがGitHub上に設置されている。トレンドマイクロ社
    * https://www.trendmicro.com/en_us/research/25/a/information-stealer-masquerades-as-ldapnightmare-poc-exploit.html
