---
title: "2026/01/11 週 セキュリティニュースメモ"
emoji: "🔖"
type: "idea"
topics: ["Security"]
published: false
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。そのため、zenn上で未公開でも、[GitHub上では確認](https://github.com/hinoshiba/zenn.dev/tree/main/articles) はできます。
* あくまで、みた週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません

# 事件事故

* Instagram、1750万アカウントの情報流出か
    * https://x.com/Malwarebytes/status/2009664994070184282?ref_src=twsrc%5Etfw%7Ctwcamp%5Etweetembed%7Ctwterm%5E2009664994070184282%7Ctwgr%5Ef62979b2a8bd0ed4a75804bc5e86055dd6a47545%7Ctwcon%5Es1_c10&ref_url=https%3A%2F%2Fgori.me%2Ffacebook%2Finstagram%2F163028
    * https://www.bleepingcomputer.com/news/security/instagram-denies-breach-amid-claims-of-17-million-account-data-leak/
    * https://haveibeenpwned.com/Breach/Instagram

# 攻撃、脅威

* 社長名で届く「LINEグループを作成してください」　迷惑メールに注意
    * https://news.yahoo.co.jp/articles/e2c31e183ef44966b958054990f725e202d9cfc4

# 脆弱性

* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2026-jan
        * https://securityonline.info/patch-tuesday-jan-2026-microsoft-fixes-114-flaws-3-zero-days/
        * https://www.securityweek.com/microsoft-patches-exploited-windows-zero-day-111-other-vulnerabilities/
    * CVE-2026-20805
        * https://www.theregister.com/2026/01/14/patch_tuesday_january_2026/
* CVE-2025-64155 FortiSIEM OSコマンドインジェクション
    * https://securityonline.info/fortinet-critical-alert-cve-2025-64155-rce-config-leaks-exposed/
    * https://www.fortiguard.com/psirt/FG-IR-25-772


## KEV

* CVE-2025-8110 Gogs Path Traversal Vulnerability
    * https://www.bleepingcomputer.com/news/security/cisa-orders-feds-to-patch-gogs-rce-flaw-exploited-in-zero-day-attacks/

# その他
* Word Kindleに送るの機能なくなる
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-is-retiring-send-to-kindle-in-word/
* Windows 11 24H2 and 25H2 で、期限切れのセキュアブート用証明書を自動的に置き換える
    * https://www.bleepingcomputer.com/news/security/microsoft-rolls-out-new-secure-boot-certificates-for-windows-devices/
