---
title: "2025/12/07 週 セキュリティニュースメモ"
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

* アスクル株式会社 / ランサムウェア攻撃の影響調査結果および安全性強化に向けた取り組みのご報告（ランサムウェア攻撃によるシステム障害関連・第 13 報）
    * https://prtimes.jp/main/html/rd/p/000000500.000021550.html

# 攻撃、脅威

# 脆弱性

* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-dec
        * https://krebsonsecurity.com/2025/12/microsoft-patch-tuesday-december-2025-edition/
        * https://www.securityweek.com/microsoft-patches-57-vulnerabilities-three-zero-days/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-december-2025-patch-tuesday-fixes-3-zero-days-57-flaws/
    * CVE-2025-54100 PowerShell iwr(Invoke-WebRequest) コマンドに、パース時にコードが実行される脆弱性。修正によりコマンド実行時に警告が表示されるようになる
        * https://www.bleepingcomputer.com/news/security/microsoft-windows-powershell-now-warns-when-running-invoke-webrequest-scripts/
* Node.js が15日に脆弱性修正バージョンの公開を予告
    * https://nodejs.org/en/blog/vulnerability/december-2025-security-releases
* CVE-2024-55947 Gogs 任意のコード実行の脆弱性
    * https://www.bleepingcomputer.com/news/security/unpatched-gogs-zero-day-rce-flaw-actively-exploited-in-attacks/
    * https://thehackernews.com/2025/12/unpatched-gogs-zero-day-exploited.html
* CVE-2025-59718 and CVE-2025-59719 FortiOS 認証bypassの脆弱性
    * https://www.securityweek.com/fortinet-patches-critical-authentication-bypass-vulnerabilities/
    * https://www.cvedetails.com/cve/CVE-2025-59718/ 
    * https://thehackernews.com/2025/12/fortinet-fortigate-under-active-attack.html
    * https://www.bleepingcomputer.com/news/security/hackers-exploit-newly-patched-fortinet-auth-bypass-flaws/
    * https://www.securityweek.com/in-the-wild-exploitation-of-fresh-fortinet-flaws-begins/

## KEV
* CVE-2025-6218 RARLAB WinRAR Path Traversal Vulnerability
* CVE-2025-62221 Microsoft Windows Use After Free Vulnerability 
* CVE-2025-58360 OSGeo GeoServer Improper Restriction of XML External Entity Reference Vulnerability 


# その他
* 日本サイバーセキュリティ産業振興コミュニティ（NCPC）設立のお知らせ
    * https://prtimes.jp/main/html/rd/p/000000197.000013310.html
* LINE ヤフー バグバウンティプログラム一時停止
    * https://bugbounty.linecorp.com/ja/
    * https://www.itmedia.co.jp/news/articles/2512/11/news092.html
        * `同プログラム参加者と同社によるバグ検証中に情報漏えいが起きたため。`
* 2025 CWE Top 25 Most Dangerous Software Weaknesses
    * https://cwe.mitre.org/top25/archive/2025/2025_cwe_top25.html
    * https://www.cisa.gov/news-events/alerts/2025/12/11/2025-cwe-top-25-most-dangerous-software-weaknesses
* Kali Linux 2025.04 release
    * https://www.bleepingcomputer.com/news/security/kali-linux-20254-released-with-3-new-tools-desktop-updates/
