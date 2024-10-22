---
title: "2024/10/20 週 セキュリティニュースメモ"
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

* 名古屋市HP サイバー攻撃により繋がりずらい状況
    * https://news.biglobe.ne.jp/topics/it/1020/00782.html
    * https://www.msn.com/ja-jp/news/national/%E5%90%8D%E5%8F%A4%E5%B1%8B%E5%B8%82%EF%BD%88%EF%BD%90%E3%81%AB%E3%82%B5%E3%82%A4%E3%83%90%E3%83%BC%E6%94%BB%E6%92%83%E3%81%8B-%E5%A4%A7%E9%87%8F%E3%81%AE%E3%82%A2%E3%82%AF%E3%82%BB%E3%82%B9%E3%81%A7%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E9%9A%9C%E5%AE%B3-%E9%96%B2%E8%A6%A7%E3%81%97%E3%81%A5%E3%82%89%E3%81%84%E7%8A%B6%E6%85%8B/ar-AA1sANIM
    * https://news.goo.ne.jp/article/yomiuri/nation/20241020-567-OYT1T50096.html
    * https://www.msn.com/ja-jp/news/national/%E5%90%8D%E5%8F%A4%E5%B1%8B%E5%B8%82%E3%81%AEhp%E3%81%8C%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0%E9%9A%9C%E5%AE%B3-%E3%82%B5%E3%82%A4%E3%83%90%E3%83%BC%E6%94%BB%E6%92%83%E3%81%AE%E5%8F%AF%E8%83%BD%E6%80%A7%E3%82%82/ar-AA1sAuYk
    * https://www.asahi.com/articles/ASSBN3S8VSBNOIPE00YM.html
    * https://news.goo.ne.jp/article/tokaitv/nation/tokaitv-20241020-1948-36940.html
    * https://www.fnn.jp/articles/-/775235
* 福岡空港などでHP障害
    * https://www.nishinippon.co.jp/item/n/1272456/
    * https://www3.nhk.or.jp/fukuoka-news/20241021/5010025938.html
* Internet Archve 攻撃者となのる主張。Gitのconfigファイルが開発サーバ上にあったことからAPIトークンを窃取とのこと
    * https://www.bleepingcomputer.com/news/security/internet-archive-breached-again-through-stolen-access-tokens/

# 脆弱性
* CVE-2024-30090 6月に修正された権限昇格の脆弱性。PoCリリース
    * https://securityonline.info/microsoft-windows-flaw-cve-2024-30090-poc-exploit-published-posing-system-privilege-threat/ 


## KEV
* CVE-2024-9537 ScienceLogic SL1 Unspecified Vulnerability

# その他

* Microsoft 引退させたハニーポットに関するブログを公開
    * https://www.bleepingcomputer.com/news/security/microsoft-creates-fake-azure-tenants-to-pull-phishers-into-honeypots/
