---
title: "2025/06/29 週 セキュリティニュースメモ"
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

* Qantas航空、サイバー攻撃
    * https://www.bleepingcomputer.com/news/security/qantas-discloses-cyberattack-amid-scattered-spider-aviation-breaches/
    * https://databreaches.net/2025/07/01/qantas-customers-involved-in-mammoth-data-breach/
* 米国、北朝鮮IT労働者スキームの仲介者を逮捕
    * https://www.theregister.com/2025/06/30/us_north_korea_workers/
    * https://thehackernews.com/2025/07/us-arrests-key-facilitator-in-north.html


# 脆弱性

* CVE-2025-32463 Linux 権限昇格。Sudo -R により。
    * https://securityonline.info/critical-sudo-flaws-cve-2025-32463-cvss-9-3-root-privilege-escalation-host-bypass-poc-available/

## KEV
* CVE-2025-48927 TeleMessage TM SGNL Initialization of a Resource with an Insecure Default Vulnerability
* CVE-2025-48928 TeleMessage TM SGNL Exposure of Core Dump File to an Unauthorized Control Sphere Vulnerability
*  CVE-2025-6543 Citrix NetScaler ADC and Gateway Buffer Overflow Vulnerability


# その他

* Cloudflare AIによるスキャンをデフォルトブロック。7/1から。
    * https://www.securityweek.com/cloudflare-puts-a-default-block-on-ai-web-scraping/
* Microsoft Authenticator パスワードマネージャ機能を8/1に終了
    * https://thehackernews.com/2025/07/microsoft-removes-password-management.html
