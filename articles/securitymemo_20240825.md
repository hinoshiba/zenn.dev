---
title: "2024/08/25 週 セキュリティニュースメモ"
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

* マクドナルドのインスタグラムアカウントがハイジャックされ仮想通貨の宣伝に利用された
    * https://securityonline.info/mcdonalds-falls-victim-to-cyberattack-instagram-hijacked-to-promote-grimace-cryptocurrency/
* KUMON、新たに計75万人以上の個人情報漏えいが判明、6月に発表した委託先のランサムウェア被害で続報
    * https://news.goo.ne.jp/article/internet_watch/trend/internet_watch-1618214.html
* KADOKAWAと交渉決裂とロ系ハッカー
    * https://www.47news.jp/11390826.html
    * https://www.at-s.com/news/article/national/1542809.html
* ＬＩＮＥ企業向けアカウント６８８件が乗っ取り被害、詐欺メッセージなどが送られた可能性。パスワードリスト型攻撃により。
    * https://www.yomiuri.co.jp/national/20240826-OYT1T50167/

# 脆弱性

* CVE-2024-6670, CVE-2024-6671, and CVE-2024-6672 Progress ネットワークモニタリングソフト(WhatsUp Gold) に、未認証のアクセスや、権限昇格の脆弱性
    * https://community.progress.com/s/article/WhatsUp-Gold-Security-Bulletin-August-2024
    * https://securityonline.info/critical-vulnerabilities-uncovered-in-progress-whatsup-gold-cve-2024-6670-cve-2024-6671/
* CVE-2024-40766 SonicWall 未認証のリソースアクセスの脆弱性
    * https://thehackernews.com/2024/08/sonicwall-issues-critical-patch-for.html
* ~CVE-2024-42992 Pandas 任意のファイルを読み取ることができる脆弱性~？
    * https://securityonline.info/critical-flaw-discovered-in-popular-python-library-pandas-no-patch-available-for-cve-2024-42992/
    * CVE拒絶
        * https://www.security-next.com/161144
* CVE-2024-45163 Mirai botnet 未認証のアクセスやDoSの脆弱性
    * https://securityonline.info/hacking-the-hacker-researcher-found-critical-flaw-cve-2024-45163-in-mirai-botnet/
* CVE-2024-43399 MobSF 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-43399-critical-zip-slip-vulnerability-discovered-in-mobile-security-framework-mobsf/
* CVE-2024-39717 Versa Director GUI 認証後の任意のファイルアップロードによる任意のコード実行の脆弱性
    * https://krebsonsecurity.com/2024/08/new-0-day-attacks-linked-to-chinas-volt-typhoon/
    * https://www.darkreading.com/cyberattacks-data-breaches/china-s-volt-typhoon-actively-exploiting-now-patched-0-day-in-versa-director-servers
    * https://www.bleepingcomputer.com/news/security/chinese-volt-typhoon-hackers-exploited-versa-zero-day-to-breach-isps-msps/
* CVE-2024-7965 GoogleChromeヒープ破壊の脆弱性。攻撃の利用を確認
    * https://www.securityweek.com/google-warns-of-exploited-chrome-vulnerability/
    * https://thehackernews.com/2024/08/google-warns-of-cve-2024-7965-chrome.html
    * https://securityonline.info/google-chrome-faces-double-blow-with-new-zero-day-flaw-exploits-cve-2024-7965-and-cve-2024-7971/
    * https://www.security-next.com/161147
* CVE-2024-6386 WordPress 多言語対応プラグイン WPML 認証済みユーザによる任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-6386-cvss-9-9-in-wpml-plugin-exposes-millions-of-wordpress-sites-to-rce-attacks/
* KEV
    * CVE-2024-38856  Apache OFBiz Incorrect Authorization Vulnerability
    * CVE-2024-39717 Versa Director Dangerous File Type Upload Vulnerability
    * CVE-2024-7971 Google Chromium V8 Type Confusion Vulnerability

# その他

* テレグラムCEO フランス当局に逮捕
    * https://jp.reuters.com/world/security/RLENG7HPDFL2HLMQIDFD6GNGDE-2024-08-25/
    * https://thehackernews.com/2024/08/telegram-founder-pavel-durov-arrested.html
    * https://www.securityweek.com/french-authorities-arrest-telegram-ceo-pavel-durov-at-a-paris-airport-french-media-report/
* Exchange Onlineにて、メールが誤ってマルウェアのタグ付がされる不具合
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-exchange-online-mistakenly-tags-emails-as-malware/
* Uber GDPR に関する罰金について、上告
    * https://www.securityweek.com/uber-to-appeal-dutch-e290-million-gdpr-fine/
    * https://securityonline.info/uber-hit-with-e290-million-gdpr-fine-by-dutch-dpa/
* notion 9/9にロシアから撤退
    * https://www.bleepingcomputer.com/news/software/notion-exits-russia-and-will-terminate-accounts-in-september/
* Windows Downgrade攻撃に用いることができるツール、WindowsDowndate リリース
    * https://www.bleepingcomputer.com/news/microsoft/windows-downdate-tool-lets-you-unpatch-windows-systems/
    * https://github.com/SafeBreach-Labs/WindowsDowndate
