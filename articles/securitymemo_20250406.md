---
title: "2025/04/06 週 セキュリティニュースメモ"
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

* ゆうちょ 7日午前9時ごろ ゆうちょダイレクト 等のシステム障害。原因調査中
    * https://www.jp-bank.japanpost.jp/news/2025/news_id002243.html
* NEXCO 中日本 ECT障害
    * https://dc2.c-nexco.co.jp/etc/
    * https://merkmal-biz.jp/post/90360/2

# 攻撃、脅威

# 脆弱性
* CVE-2025-31115 XZ Utils 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2025-31115-xz-utils-hit-again-with-high-severity-multithreaded-decoder-bug/
* CVE-2025-29987 Dell PowerProtect root権限でのこーどじっこう
    * https://securityonline.info/unpatched-dell-powerprotect-systems-vulnerable-to-remote-compromise/
* CVE-2024-48887 FortiSwitch 未認証の接続
    * https://thehackernews.com/2025/04/fortinet-urges-fortiswitch-upgrades-to.html
    * https://securityonline.info/fortinet-critical-unverified-password-change-flaw-in-fortiswitch/
    * https://www.bleepingcomputer.com/news/security/critical-fortiswitch-flaw-lets-hackers-change-admin-passwords-remotely/
    * https://www.securityweek.com/fortinet-patches-critical-fortiswitch-vulnerability/
* CVE-2024-53197 Android 権限昇格の脆弱性
    * https://www.darkreading.com/vulnerabilities-threats/android-zero-day-bugs-active-exploit
    * https://www.securityweek.com/android-update-patches-two-exploited-vulnerabilities/
    * https://thehackernews.com/2025/04/google-releases-android-update-to-patch.html
* CVE-2025-27520 BentoML RCEの脆弱性 
    * https://securityonline.info/cve-2025-27520-critical-bentoml-flaw-allows-full-remote-code-execution-exploit-available/
* CVE-2024-12556 Kibana Code Injection
    * https://securityonline.info/kibana-code-injection-vulnerability-prototype-pollution-threat-cve-2024-12556/
* WindowsUpdate
    * info
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://msrc.microsoft.com/update-guide/releaseNote/2025-Apr
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-april-2025-patch-tuesday-fixes-exploited-zero-day-134-flaws/
        * https://thehackernews.com/2025/04/microsoft-patches-126-flaws-including.html
        * https://securityonline.info/microsoft-april-2025-patch-tuesday-critical-security-updates-and-zero-day-exploits/
    * CVE-2025-29824
        * https://www.microsoft.com/en-us/security/blog/2025/04/08/exploitation-of-clfs-zero-day-leads-to-ransomware-activity/
        * https://www.bleepingcomputer.com/news/security/microsoft-windows-clfs-zero-day-exploited-by-ransomware-gang/
* Amazon EC2 SSM Agent 権限昇格の脆弱性が修正
    * https://thehackernews.com/2025/04/amazon-ec2-ssm-agent-flaw-patched-after.html

## KEV
* CVE-2025-22457 Ivanti Connect Secure, Policy Secure and ZTA Gateways Stack-Based Buffer Overflow Vulnerability
    * https://securityonline.info/ivanti-zero-day-cve-2025-22457-exploit-details-released/
* CVE-2025-31161 CrushFTP Authentication Bypass Vulnerability
* CVE-2024-53197 Linux Kernel Out-of-Bounds Access Vulnerability
* CVE-2024-53150 Linux Kernel Out-of-Bounds Read Vulnerability


# その他
* 4月の月次パッチでWindowsHelloが一部使えなくなった
    * https://www.theregister.com/2025/04/09/microsoft_hello_patch/
* Windows, 新しいセキュリティ機能により、`C:\inetpub` フォルダが作成されるとのこと
    * https://www.bleepingcomputer.com/news/microsoft/windows-11-april-update-unexpectedly-creates-new-inetpub-folder/
    * https://www.bleepingcomputer.com/news/security/microsoft-windows-inetpub-folder-created-by-security-fix-dont-delete/
    * https://www.theregister.com/2025/04/14/windows_update_inetpub/
    * https://www.bitdefender.com/en-us/blog/hotforsecurity/microsoft-april-2025-security-update-creates-empty-inetpub-folder-you-shouldnt-delete
