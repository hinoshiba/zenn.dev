---
title: "2024/08/11 週 セキュリティニュースメモ"
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

# 脆弱性

* CVE-2024-38200 MicrosoftOfficeを通じて、NTLMハッシュを窃取する脆弱性。機能アップデートで配布済み。最終盤は、8月のWindowsUpdateで配布予定
    * https://www.bleepingcomputer.com/news/security/microsoft-discloses-unpatched-office-flaw-that-exposes-ntlm-hashes/
    * https://securityonline.info/cve-2024-38200-zero-day-vulnerability-in-microsoft-office-a-call-for-urgent-action/
* CVE-2024-7589 FreeBSD 系のOpenSSH 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-7589-openssh-pre-authentication-vulnerability-in-freebsd-exposes-systems-to-rce/
    * https://thehackernews.com/2024/08/freebsd-releases-urgent-patch-for-high.html
* CVE-2024-6768 Windows 11/10 CLFSによるBSoD
    * https://www.darkreading.com/vulnerabilities-threats/clfs-bug-crashes-even-updated-windows-10-11-systems
* Microsoft研究者、OpenVPNに対する脆弱性を用いた攻撃チェーンにて、RCEのデモを実施。BlachHat 2024にて
    * https://www.microsoft.com/en-us/security/blog/2024/08/08/chained-for-attack-openvpn-vulnerabilities-discovered-leading-to-rce-and-lpe/
    * https://www.securityweek.com/microsoft-warns-of-openvpn-vulnerabilities-potential-for-exploit-chains/

# その他

* Windows 11 22H2 EOSまであと60日。(2024/10/08迄)
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-11-22h2-reaches-end-of-support-in-60-days/
* Microsoft Paint 3D 今年11月に削除予定とのこと
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-is-killing-the-windows-paint-3d-app-after-8-years/
* Google ロシアへの広告支払いの最後を実施
    * https://www.bleepingcomputer.com/news/google/google-deactivates-russian-adsense-accounts-sends-final-payments/
