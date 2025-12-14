---
title: "2025/11/30 週 セキュリティニュースメモ"
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

* 17歳男子高校生、生成AIを使った「快活CLUB」へのサイバー攻撃で逮捕 724万件の個人情報流出
    * https://news.yahoo.co.jp/articles/43df98da5cc03d4eb499d78e47c2d18c63d108d7
    * https://news.ntv.co.jp/category/society/ce9f4c1e4861492c9373932d16f7443f
* ASKUL Webサイトでの注文を12/3 に復旧
    * https://pdf.irpocket.com/C0032/VowW/kiU3/UgoY.pdf
    * https://news.mynavi.jp/techplus/article/20251203-3755740/
* 日本検定協会 サイバー攻撃を確認
    * https://www.shinken.or.jp/archives/infomation/14909
    * https://www.security-next.com/177719

# 攻撃、脅威

# 脆弱性

* CVE-2025-60718 Windows 権限昇格の脆弱性、PoCリリース
    * https://securityonline.info/poc-exploit-releases-for-cve-2025-60718-windows-administrator-protection-elevation-of-privilege-vulnerability/
* CVE-2025-55182 CVE-2025-66478 React2Shell
    * https://react2shell.com/
    * https://www.securityweek.com/react2shell-in-the-wild-exploitation-expected-for-critical-react-vulnerability/
    * https://www.bleepingcomputer.com/news/security/critical-react2shell-flaw-in-react-nextjs-lets-hackers-run-javascript-code/
    * https://www.security-next.com/177961
    * https://thehackernews.com/2025/12/critical-react2shell-flaw-added-to-cisa.html
    * https://www.bleepingcomputer.com/news/security/react2shell-flaw-exploited-to-breach-30-orgs-77k-ip-addresses-vulnerable/
    * https://thehackernews.com/2025/12/critical-react2shell-flaw-added-to-cisa.html
    * https://www.bleepingcomputer.com/news/security/react2shell-critical-flaw-actively-exploited-in-china-linked-attacks/
    * https://www.securityweek.com/react2shell-attacks-linked-to-north-korean-hackers/
    * https://www.lac.co.jp/lacwatch/alert/20251209_004572.html
    * https://securityonline.info/critical-react2shell-vulnerability-cve-2025-55182-analysis-surge-in-attacks-targeting-rsc-enabled-services-worldwide/
    * https://thehackernews.com/2025/12/new-react-rsc-vulnerabilities-enable.html
    * https://thehackernews.com/2025/12/react2shell-exploitation-escalates-into.html
* CVE-2025-66476 Vim for Windows コード実行の脆弱性
    * https://www.openwall.com/lists/oss-security/2025/12/02/5


## KEV

* CVE-2021-26828 OpenPLC ScadaBR Unrestricted Upload of File with Dangerous Type Vulnerability 

# その他
* MDE ポータルの停止により脅威ハンティングが一時停止
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-defender-portal-outage-blocks-access-to-security-alerts/
    * https://admin.microsoft.com/#/MessageCenter/:/messages/DZ1191468
* Cloudflare 障害 React2Shellの対応のため
    * https://www.bleepingcomputer.com/news/technology/cloudflare-down-websites-offline-with-500-internal-server-error/
    * https://www.securityweek.com/cloudflare-outage-caused-by-react2shell-mitigations/
    * https://www.bleepingcomputer.com/news/security/cloudflare-blames-todays-outage-on-emergency-react2shell-patch/
* インド通信省、スマホに政府アプリのインストールを義務化するも2日で撤回
    * https://news.mynavi.jp/techplus/article/20251205-3760108/
* Let's Encrypto の証明書の期間が、90日から45日に。
    * https://letsencrypt.org/2025/12/02/from-90-to-45
    * https://news.mynavi.jp/techplus/article/20251205-3760801/
