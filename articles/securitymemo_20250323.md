---
title: "2025/03/23 週 セキュリティニュースメモ"
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
    * https://securityonline.info/vmware-tools-for-windows-hit-by-cve-2025-22230-auth-bypass-flaw/
* WindowsがNTLMの脆弱性。非公式パッチあり
    * https://www.bleepingcomputer.com/news/security/new-windows-zero-day-leaks-ntlm-hashes-gets-unofficial-patch/
* CVE-2025-1974 Ingress-Nginx Controller k8s 管理が奪われる脆弱性
    * https://www.theregister.com/2025/03/25/kubernetes_flaw_rce_risk/
    * https://securityonline.info/cve-2025-1974-cvss-9-8-ingress-nginx-flaws-threaten-mass-kubernetes-compromise/
    * https://x.com/carlos_crowsec/status/1904939487224050162
    * https://securityonline.info/researcher-drops-poc-for-9-8-cvss-ingress-nginx-cve-2025-1974-flaw-in-kubernetes/
* CVE-2025-0927 Linuxカーネル権限昇格の脆弱性。PoCあり
    * https://securityonline.info/cve-2025-0927-public-exploit-released-for-linux-kernel-privilege-escalation-bug/
* CVE-2025-2783 Google Chrome ZeroDayがAPTにより使われている
    * https://www.darkreading.com/cyberattacks-data-breaches/google-patches-chrome-zero-day-exploited-apt
    * https://www.bleepingcomputer.com/news/security/google-fixes-chrome-zero-day-exploited-in-espionage-campaign/
    * https://thehackernews.com/2025/03/zero-day-alert-google-releases-chrome.html
    * https://www.securityweek.com/google-patches-chrome-sandbox-escape-zero-day-caught-by-kaspersky/
    * https://securityonline.info/cve-2025-2783-chrome-zero-day-exploited-in-state-sponsored-espionage-campaign/
* CVE-2025-2857 Firefox Sandbox escape
    * https://securityonline.info/cve-2025-2857-new-firefox-sandbox-escape-emerges-following-active-exploitation-of-cve-2025-2783/
    * https://www.bleepingcomputer.com/news/security/mozilla-warns-windows-users-of-critical-firefox-sandbox-escape-flaw/
    * https://www.theregister.com/2025/03/28/google_kaspersky_mozilla/
    * https://thehackernews.com/2025/03/mozilla-patches-critical-firefox-bug.html
* CVE-2025-2255 GitLab XSS
    * https://securityonline.info/gitlab-alert-patch-now-xss-privilege-escalation-risks/
* CVE-2025-2848 Synology Mail Server 設定改ざんの脆弱性
    * https://securityonline.info/cve-2025-2848-synology-mail-server-vulnerability-allows-remote-configuration-tampering/
* CVE-2025-20229 Splunk RCE
    * https://securityonline.info/splunk-alert-rce-and-data-leak-vulnerabilities-threaten-platforms/


## KEV
* CVE-2025-30154 reviewdog action-setup GitHub Action Embedded Malicious Code Vulnerability
* CVE-2019-9874 Sitecore CMS and Experience Platform (XP) Deserialization Vulnerability
* CVE-2019-9875 Sitecore CMS and Experience Platform (XP) Deserialization Vulnerability
* CVE-2025-2783 Google Chromium Mojo Sandbox Escape Vulnerability


# その他

* Cloudflare api.cloudflare.com に対するアクセスをHTTPSのみとする
    * https://www.bleepingcomputer.com/news/security/cloudflare-now-blocks-all-unencrypted-traffic-to-its-api-endpoints/
    * https://securityonline.info/cloudflare-pulls-the-plug-on-http-api-now-https-only/
* Cloudflare Object Storageサービス R2 1hダウン
    * https://securityonline.info/r2-down-cloudflares-object-storage-hit-by-1-hour-outage/
* Chromeのインストーラ、誤ってx86にarmを配布
    * https://securityonline.info/chrome-installer-bug-arm-version-delivered-to-x86-users/
