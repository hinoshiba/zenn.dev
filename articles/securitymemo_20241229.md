---
title: "2024/12/29 週 セキュリティニュースメモ"
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

* りそな銀行 繋がりづらい状態
    * https://www.yomiuri.co.jp/national/20241230-OYT1T50097/
    * https://news.goo.ne.jp/picture/nation/20241230-567-OYT1T50097.html
    * https://www.sankei.com/article/20241230-DOWAMZU7NVPK7HNNRWCRFKBPJA/
* みずほ銀行 繋がりづらい状態
    * https://www.yomiuri.co.jp/economy/20241231-OYT1T50045/

# 攻撃、脅威

* 35個のChromeExtensionがハッキングを受け、ユーザのデータを盗むアップデートが行われる
    * https://thehackernews.com/2024/12/16-chrome-extensions-hacked-exposing.html
    * https://www.bleepingcomputer.com/news/security/new-details-reveal-how-hackers-hijacked-35-google-chrome-extensions/
    * https://www.extensiontotal.com/cyberhaven-incident-live
    * https://www.bleepingcomputer.com/news/security/malicious-browser-extensions-are-the-next-frontier-for-identity-attacks/
    * https://news.mynavi.jp/techplus/article/20250106-3101219/

# 脆弱性

* CVE-2024-49113 12月に修正されたWindowsLDAPの脆弱性、PoCリリース
    * https://www.securityweek.com/exploit-code-published-for-potentially-dangerous-windows-ldap-vulnerability/
    * https://thehackernews.com/2025/01/ldapnightmare-poc-exploit-crashes-lsass.html
    * https://securityonline.info/poc-exploit-released-for-zero-click-vulnerability-cve-2024-49112-in-windows/
* CVE-2025-22275 iTerm2 ユーザの入出力がサーバ上に保存されてしまう脆弱性
    * https://securityonline.info/iterm2-patches-critical-security-vulnerability-exposing-user-input-and-output/
* CVE-2024-21182 2024/07月に公開されたWebLogicの脆弱性、PoCリリース
    * https://securityonline.info/cve-2024-21182-poc-exploit-code-published-for-severe-weblogic-flaw/

## KEV
* CVE-2024-3393 Palo Alto Networks PAN-OS Malformed DNS Packet Vulnerability

# その他

