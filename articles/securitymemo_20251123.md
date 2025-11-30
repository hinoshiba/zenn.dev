---
title: "2025/11/23 週 セキュリティニュースメモ"
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

* OpenAI が利用するMixpanel の情報侵害によりOpenAIの登録メールアドレス等の情報が流出
    * https://openai.com/index/mixpanel-incident/
* アサヒグループ / サイバー攻撃による情報漏えいに関する調査結果と今後の対応について
    * https://www.asahigroup-holdings.com/newsroom/detail/20251127-0104.html
    * https://www.bleepingcomputer.com/news/security/japanese-beer-giant-asahi-says-data-breach-hit-15-million-people/
* ASKUL Webサイトの注文を12月第一週で復旧対応中
    * https://pdf.irpocket.com/C0032/VowW/wP9e/bCCh.pdf


# 攻撃、脅威

* WindowsUpdateを語るClickFix
    * https://www.theregister.com/2025/11/24/clickfix_attack_infostealers_images/
    * https://www.bleepingcomputer.com/news/security/clickfix-attack-uses-fake-windows-update-screen-to-push-malware/


# 脆弱性

* CVE-2025-65108 md-to-pdf コード実行の脆弱性
    * https://securityonline.info/critical-markdown-to-pdf-flaw-cve-2025-65108-cvss-10-0-allows-rce-via-js-injection-in-markdown-front-matter/
* e CVE-2025-59366 ASUS Router 認証bypass
    * https://www.bleepingcomputer.com/news/security/asus-warns-of-new-critical-auth-bypass-flaw-in-aicloud-routers/
    * https://www.asus.com/security-advisory/



## KEV
* CVE-2021-26829 OpenPLC ScadaBR Cross-site Scripting Vulnerability 


# その他
* 8月以降のWindowsUpdateによって Passwordログインボタンがそのままだと表示されない不具合, MSは修正中
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-updates-hide-password-icon-on-lock-screen/
