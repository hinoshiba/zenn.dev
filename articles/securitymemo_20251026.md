---
title: "2025/10/26 週 セキュリティニュースメモ"
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

# 攻撃、脅威

* QilinがWSLを介してELFを実行し、暗号化を行う手法
    * https://www.bleepingcomputer.com/news/security/qilin-ransomware-abuses-wsl-to-run-linux-encryptors-in-windows/

# 脆弱性

* CVE-2025-62725 Docker Compose Path Traversal
    * https://securityonline.info/docker-compose-path-traversal-cve-2025-62725-allows-arbitrary-file-overwrite-via-oci-artifacts/
    * https://www.theregister.com/2025/10/30/docker_compose_desktop_flaws/


## KEV
* CVE-2025-6204 Dassault Systèmes DELMIA Apriso Code Injection Vulnerability
* CVE-2025-6205 Dassault Systèmes DELMIA Apriso Missing Authorization Vulnerability
* CVE-2025-24893 XWiki Platform Eval Injection Vulnerability
* CVE-2025-41244 Broadcom VMware Aria Operations and VMware Tools Privilege Defined with Unsafe Actions Vulnerability


# その他
* Windows BSOD 時にメモリスキャンができるプロンプトを追加中
    * https://www.bleepingcomputer.com/news/microsoft/windows-will-soon-prompt-for-memory-scans-after-bsod-crashes/
