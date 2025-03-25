---
title: "2025/03/23 週 セキュリティニュースメモ"
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

* 新規アプリ登録者のメアド流出、システム設定ミスで - マクドナルド
    * https://www.security-next.com/168437

# 攻撃、脅威

# 脆弱性

* CVE-2025-1758 Progress Kemp LoadMaster RCE
    * https://securityonline.info/cve-2025-1758-critical-buffer-overflow-in-kemp-loadmaster-opens-door-to-remote-code-execution/
* CVE-2025-29927 NextJS 認証bypassの脆弱性
    * https://securityonline.info/urgent-patch-your-next-js-for-authorization-bypass-cve-2025-29927/
* CVE-2025-22230 VMWare Windows Vmware tools 認証bypassの脆弱性
    * https://www.bleepingcomputer.com/news/security/broadcom-warns-of-authentication-bypass-in-vmware-windows-tools/
    * https://www.securityweek.com/vmware-patches-authentication-bypass-flaw-in-windows-tools-suite/
* WindowsがNTLMの脆弱性。非公式パッチあり
    * https://www.bleepingcomputer.com/news/security/new-windows-zero-day-leaks-ntlm-hashes-gets-unofficial-patch/
* CVE-2025-1974 Ingress-Nginx Controller k8s 管理が奪われる脆弱性
    * https://www.theregister.com/2025/03/25/kubernetes_flaw_rce_risk/
    * https://securityonline.info/cve-2025-1974-cvss-9-8-ingress-nginx-flaws-threaten-mass-kubernetes-compromise/
* CVE-2025-0927 Linuxカーネル権限昇格の脆弱性。PoCあり
    * https://securityonline.info/cve-2025-0927-public-exploit-released-for-linux-kernel-privilege-escalation-bug/

## KEV
* CVE-2025-30154 reviewdog action-setup GitHub Action Embedded Malicious Code Vulnerability


# その他

* Cloudflare api.cloudflare.com に対するアクセスをHTTPSのみとする
    * https://www.bleepingcomputer.com/news/security/cloudflare-now-blocks-all-unencrypted-traffic-to-its-api-endpoints/
    * https://securityonline.info/cloudflare-pulls-the-plug-on-http-api-now-https-only/
