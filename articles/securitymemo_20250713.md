---
title: "2025/07/13 週 セキュリティニュースメモ"
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

* Geminiによるメール要約を使いフィッシングを生成するテクニック
    * https://www.bleepingcomputer.com/news/security/google-gemini-flaw-hijacks-email-summaries-for-phishing/
    * https://www.darkreading.com/remote-workforce/google-gemini-ai-bug-invisible-malicious-prompts
* ユーロポールが「オペレーション・イーストウッド」でハッカー集団NoName057(16)を壊滅、ウクライナへのDDoS攻撃を阻止
    * https://thehackernews.com/2025/07/europol-disrupts-noname05716-hacktivist.html
* 警察庁サイバー特別捜査部が“世界初”の「復元ツール」を開発　ランサムウェア「Phobos」「8Base」の暗号化された被害データを完全復活
    * https://topics.smt.docomo.ne.jp/article/tbs/nation/tbs-2052812


# 脆弱性

* CVE-2025-20337 Cisco ISE 未認証のユーザによるファイルのアップロードやコード実行
    * https://www.bleepingcomputer.com/news/security/max-severity-cisco-ise-bug-allows-pre-auth-command-execution-patch-now/
    * https://securityonline.info/critical-cisco-ise-flaw-cve-2025-20337-cvss-10-0-allows-unauthenticated-root-rce-patch-immediately/

## KEV
* CVE-2025-47812 Wing FTP Server Improper Neutralization of Null Byte or NUL Character Vulnerability
* CVE-2025-25257 Fortinet FortiWeb SQL Injection Vulnerability


# その他

* UK NCSC VRIという外部サイバーセキュリティ専門家との脆弱性研究イニシアチブを発表
    * https://www.bleepingcomputer.com/news/security/uk-launches-vulnerability-research-program-for-external-experts/
* Microsoft Skype for business 2015, 2019 の2026/04までの有償セキュリティサポート を最終リリース
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/microsoft-rolls-out-final-six-month-security-extension-for-legacy-exchange-and-skype-users* Cloudflare 7月14日の1.1.1.1の障害は、サイバー攻撃ではないと表明
    * https://www.bleepingcomputer.com/news/security/cloudflare-says-1111-outage-not-caused-by-attack-or-bgp-hijack/
