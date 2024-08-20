---
title: "2024/08/18 週 セキュリティニュースメモ"
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

* セイコーエプソン 不正アクセス。現時点で流出は確認されていない
    * https://corporate.epson/ja/news/2024/240808.html
    * https://scan.netsecurity.ne.jp/article/2024/08/14/51470.html
* 機密データへの不正アクセスを防止・報告しなかったとしてT-Mobileに80億円超の罰金
    * https://gigazine.net/news/20240817-cfius-tmobile-60-million-usd-penalty/

# 脆弱性
* macOS上で動作するOfficeソフトに、ライブラリインジェクションの脆弱性があるとCiscoTalosリサーチャ報告。Microsoftは修正予定無しとのこと
    * https://www.darkreading.com/remote-workforce/multiple-microsoft-apps-for-macos-vuln-to-malicious-library-injection-attacks
    * https://www.theregister.com/2024/08/19/cisco_talos_microsoft_macos/
* CVE-2024-7646 k8s ingress-nginx 認証bypass
    * https://securityonline.info/cve-2024-7646-a-threat-to-kubernetes-clusters-running-ingress-nginx/
* KEV
    * CVE-2024-23897 Jenkins Command Line Interface (CLI) Path Traversal Vulnerability
        * https://www.bleepingcomputer.com/news/security/cisa-warns-of-jenkins-rce-bug-exploited-in-ransomware-attacks/
        * https://www.security-next.com/160926

# その他
* Windows11 24H2 より、BitLockerがデフォルトに。
    * https://securityonline.info/windows-11-24h2-microsoft-enforces-device-encryption-by-default/
