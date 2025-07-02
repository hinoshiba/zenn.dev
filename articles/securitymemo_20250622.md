---
title: "2025/06/22 週 セキュリティニュースメモ"
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


# 脆弱性

* CVE-2025-49384 トレンドマイクロ ウイルスバスター 他のローカルユーザにファイルを削除される可能性
    * https://news.yahoo.co.jp/articles/322d3894cc002c34a626e4d301abea0210df8156
* CVE-2025-2135 Kibana RCEの脆弱性
    * https://securityonline.info/critical-kibana-flaws-cve-2025-2135-cvss-9-9-allows-heap-corruption-open-redirect-also-patched/
* CVE-2025-36537 TeamViewer 権限昇格の脆弱性
    * https://securityonline.info/teamviewer-remote-management-bug-cve-2025-36537-enables-privilege-escalation/
* CVE-2025-4517 Python tar関係、任意の箇所へのファイル書き込み
    * https://securityonline.info/critical-python-tarfile-flaw-cve-2025-4517-cvss-9-4-arbitrary-file-write-poc-available/
* CVE-2024-56731 Gogs パストラバーサルの脆弱性
    * https://securityboulevard.com/2025/06/gogs-remote-command-execution-vulnerability-cve-2024-56731/
    * https://www.security-next.com/171710
* CVE-2025-6218 WinRAR 任意のコード実行
    * https://www.security-next.com/171678
    * https://www.bleepingcomputer.com/news/security/winrar-patches-bug-letting-malware-launch-from-extracted-archives/
* CVE-2025-20281 Cisco ISE RCE
    * https://www.theregister.com/2025/06/26/patch_up_cisco_fixes_two/
    * https://www.bleepingcomputer.com/news/security/cisco-warns-of-max-severity-rce-flaws-in-identity-services-engine/
    * https://thehackernews.com/2025/06/critical-rce-flaws-in-cisco-ise-and-ise.html
* CVE-2025-3509 GHE RCE
    * https://www.securityweek.com/code-execution-vulnerability-patched-in-github-enterprise-server/
* CVE-2025-49144 Notepad++ インストーラによる不具合で権限昇格の可能性
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/notepad-vulnerability-lets-attackers-take-full-system-control-poc-released
# その他

* Cloudflare Orange Meetsをオープンソース化
    * https://www.bleepingcomputer.com/news/security/cloudflare-open-sources-orange-meets-with-end-to-end-encryption/
* Windows 11 25H2 1Passwordの統合をよりシームレスなものに
    * https://securityonline.info/windows-11-25h2-dev-build-unveils-deeper-1password-integration-for-seamless-passkey-management/
* Apple 公衆Wifiのログインを1度だけとするCaptiveAssitを開発中
    * https://securityonline.info/ios-26-unveils-captive-assist-seamless-public-wi-fi-login-across-all-your-apple-devices/
    * https://securityonline.info/ios-26-unveils-new-wi-fi-sync-auto-login-for-public-networks-across-all-your-apple-devices/
* Windows Snipping Toolにて、アニメーションGIFの作成が可能となる
    * https://www.bleepingcomputer.com/news/microsoft/windows-snipping-tool-now-lets-you-create-animated-gif-recordings/
