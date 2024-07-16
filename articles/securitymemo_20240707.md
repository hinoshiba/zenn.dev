---
title: "2024/07/07 週 セキュリティニュースメモ"
emoji: "🎋"
type: "tech"
topics: ["Security"]
published: true
---

# はじめに
* 自身なりに気になったセキュリティ情報の **私のメモ** です
* 毎週日曜日起点で作成し、土曜日まで、その週の記事を更新し続けます
    * zennでの公開は、翌週の記事を作成したタイミングで実施します。ただし、GitHub上では常にpublicです。早いのはGitHubです
* あくまで、発見した週に記入します(タイトルが近い場合は、最初に見つけた週)
    * 1週間以上前の出来事は、極力日付を入れる気持ちではいますが、確実性はありません
    * 今週にhinoshibaが見つけたニュースである事に留意ください
* 実質的には、[セキュリティは楽しいかね？ Part 2](https://negi.hatenablog.com/) のような事ができるようになったらいいなと、個人的に真似をして、個人的に漏れチェック等に使います

# 事件事故

# 攻撃、脅威

* 2023/10 のJAXA不正アクセス、起点は、VPN
    * https://www.security-next.com/159383
    * https://www.jaxa.jp/press/2024/07/20240705-2_j.html
    * https://www.theregister.com/2024/07/11/jaxa_m365_zeroday_attacks/
* 富士通 2024/03月のサイバー攻撃を報告
    * https://news.mynavi.jp/techplus/article/20240710-2983063/
    * https://www.itmedia.co.jp/news/articles/2407/10/news110.html
* 東京海上日動 業務委託先ランサムウェア被害
    * https://www.nikkei.com/nkd/company/article/?DisplayType=11&ng=DGXZRSP674679_Q4A710C2000000&nik_code=0070501
    * https://newsdig.tbs.co.jp/articles/-/1287199
    * https://article.auone.jp/detail/1/3/6/333_6_r_20240710_1720617048954903
    * https://www.yomiuri.co.jp/national/20240710-OYT1T50177/
* AT&T 不正アクセスにより顧客情報やメッセージテキスト漏洩
    * https://thehackernews.com/2024/07/at-confirms-data-breach-affecting.html
    * https://www.darkreading.com/cyberattacks-data-breaches/att-breach-may-also-impact-millions-of-boost-cricket-h2o-customers
    * https://www.cisa.gov/news-events/alerts/2024/07/12/att-discloses-breach-customer-data
    * https://www.theregister.com/2024/07/12/att_110_million_call_text_logs/
    * https://securityboulevard.com/2024/07/att-snowflake-breach-richixbw/
    * https://databreaches.net/2024/07/12/att-says-new-hack-includes-records-of-customer-calls-texts/
    * https://sp.m.jiji.com/article/show/3284310
    * https://www.wired.com/story/atandt-paid-hacker-300000-to-delete-stolen-call-records/

# 脆弱性
* CVE-2024-34750 Apache Tomcat DoSの脆弱性
    * https://jvn.jp/vu/JVNVU90387090/index.html
    * https://www.security-next.com/159421
* CVE-2024-36991 Splunk パスとラバーサルの脆弱性
    * https://nvd.nist.gov/vuln/detail/CVE-2024-36991
    * https://github.com/bigb0x/CVE-2024-36991
* CVE-2024-39202 D-Link Router RCE PoCあり
    * https://gist.github.com/Swind1er/40c33f1b1549028677cb4e2e5ef69109
* CVE-2024-39349 Synology Camera 任意のコード実行の脆弱性
    * https://securityonline.info/cve-2024-39349-cvss-9-8-critical-vulnerability-in-synology-surveillance-cameras/
* CVE-2024-5441 WordPress Plugin Modern Events Calendar RCE
    * https://www.bleepingcomputer.com/news/security/hackers-target-wordpress-calendar-plugin-used-by-150-000-sites/
* CVE-2024-3596 RADIUS プロトコル MitMの可能性
    * https://www.cvedetails.com/cve/CVE-2024-3596/?q=CVE-2024-3596
    * https://kb.cert.org/vuls/id/456537
    * https://securityboulevard.com/2024/07/blast-radius-mitm-md5-richixbw/
* CVE-2024-6409 OpenSSH RCEの脆弱性
    * https://securityonline.info/cve-2024-6409-new-remote-code-execution-vulnerability-in-openssh/
    * https://www.security-next.com/159488
    * https://thehackernews.com/2024/07/new-openssh-vulnerability-discovered.html
    * https://www.theregister.com/2024/07/11/openssh_bug_in_rhel_9/
* CVE-2024-5910 PaloAlto Palo Alto Networks Expedition アカウントが盗まれる可能性
    * https://thehackernews.com/2024/07/palo-alto-networks-patches-critical.html
    * https://securityonline.info/cve-2024-5910-critical-vulnerability-threatens-palo-alto-networks-expedition/
* CVE-2024-22274 vCentor リモートから乗っ取られる可能性 PoC 公開
    * https://securityonline.info/vmware-vcenter-server-rce-cve-2024-22274-poc-exposes-systems-to-remote-takeover/
* CVE-2024-5491 CVE-2024-5492 NetScaler ADC and NetScaler Gateway Security Bulletin 未認証のユーザが他ユーザを誘導する可能性やDoS
    * https://support.citrix.com/article/CTX677944/netscaler-adc-and-netscaler-gateway-security-bulletin-for-cve20245491-and-cve20245492%20%20
* CVE-2024-34123 Adobe Premiere Pro  信頼できないPATH探索の脆弱性
    * https://helpx.adobe.com/security/products/premiere_pro/apsb24-46.html
    * https://www.securityweek.com/adobe-issues-critical-patches-for-multiple-products-warns-of-code-execution-risks/
* CVE-2024-6385 GitLab 異なるユーザでパイプラインを実行できる脆弱性
    * https://www.bleepingcomputer.com/news/security/gitlab-warns-of-critical-bug-that-lets-attackers-run-pipelines-as-an-arbitrary-user/
    * https://www.securityweek.com/gitlab-ships-update-for-critical-pipeline-execution-vulnerability/
    * https://thehackernews.com/2024/07/gitlab-patches-critical-flaw-allowing.html
    * https://securityonline.info/gitlab-patches-critical-security-vulnerability-cve-2024-6385-urges-immediate-upgrade/
    * https://www.darkreading.com/application-security/-gitlab-sends-users-scrambling-again-with-new-ci-cd-pipeline-takeover-vuln
    * https://www.cvedetails.com/cve/CVE-2024-6385/?q=CVE-2024-6385
* CVE-2024-22280 VMware Aria Automation に対するSQLi
    * https://www.securityweek.com/vmware-patches-critical-sql-injection-flaw-in-aria-automation/
    * https://support.broadcom.com/web/ecx/support-content-notification/-/external/content/SecurityAdvisories/0/24598
    * https://securityaffairs.com/165560/security/vmware-aria-automation-critical-sql-injection.html
* CISA OSCommand Inectionの脆弱性に警告 CVE-2024-20399, CVE-2024-3400, CVE-2024-21887) to
    * https://www.cisa.gov/news-events/alerts/2024/07/10/cisa-and-fbi-release-secure-design-alert-eliminating-os-command-injection-vulnerabilities
* CVE-2024-6411 WordPressPlubin ProfileGrid 権限昇格の怖
    * https://malware.news/t/7-000-wordpress-sites-affected-by-privilege-escalation-vulnerability-in-profilegrid-wordpress-plugin/83859
    * https://wordpress.org/plugins/profilegrid-user-profiles-groups-and-communities/
* CVE-2024-26015 FortiOS 細工されたIPアドレスによってブロックリストをbypassできる脆弱性
    * https://www.fortiguard.com/psirt/FG-IR-23-446
    * https://www.security-next.com/159516
* CVE-2024-4879 ServiceNow Jelly template Injectionによるコード実行
    * https://support.servicenow.com/kb?id=kb_article_view&sysparm_article=KB1645154
* CVE-2024-39520 Juniper JunOS 権限昇格の脆弱性
    * https://supportportal.juniper.net/s/article/2024-07-Security-Bulletin-Junos-OS-Evolved-Multiple-CLI-parameter-processing-issues-allowing-privilege-escalation-resolved?language=en_US
    * https://securityonline.info/juniper-junos-os-evolved-vulnerabilities-enable-root-level-compromise/
* PSV-2023-0122 NETGEAR router XSS
    * https://www.bleepingcomputer.com/news/security/netgear-warns-users-to-patch-authentication-bypass-xss-router-flaws/
    * https://kb.netgear.com/000066264/Security-Advisory-for-Stored-Cross-Site-Scripting-on-Some-Routers-PSV-2023-0122
* PSV-2023-0138 NETGEAR 認証bypass
    * https://www.bleepingcomputer.com/news/security/netgear-warns-users-to-patch-authentication-bypass-xss-router-flaws/
    * https://kb.netgear.com/000066265/Security-Advisory-for-Authentication-Bypass-on-Some-Cable-Modem-Routers-PSV-2023-0138
* CVE-2024-39202 D-Linkルータ RCE
    * https://securityonline.info/cve-2024-39202-rce-flaw-found-in-d-link-dir-823x-firmware-patch-in-development/
* WindowsUpdate
    * info
        * https://www.securityweek.com/microsoft-warns-of-windows-hyper-v-zero-day-being-exploited/
        * https://www.bleepingcomputer.com/news/microsoft/microsoft-july-2024-patch-tuesday-fixes-142-flaws-4-zero-days/
        * https://msrc.microsoft.com/update-guide/releaseNote/2024-Jul
        * https://msrc.microsoft.com/update-guide/vulnerability
        * https://thehackernews.com/2024/07/microsofts-july-update-patches-143.html
        * https://securityboulevard.com/2024/07/patch-tuesday-update-july-2024/
        * https://www.theregister.com/2024/07/10/july_2024_patch_tuesday/
        * https://msrc.microsoft.com/blog/2024/07/202407-security-update/
    * publicly disclosed / exploited
        * CVE-2024-37985 Arm: CVE-2024-37985 Systematic Identification and Characterization of Proprietary Prefetchers
        * CVE-2024-35264 .NET and Visual Studio Remote Code Execution Vulnerability
        * CVE-2023-38545 Hackerone: CVE-2023-38545 SOCKS5 heap buffer overflow
        * CVE-2023-24932 Secure Boot Security Feature Bypass Vulnerability
        * CVE-2024-38112 Windows MSHTML Platform Spoofing Vulnerability
            * 1年以上悪用されていた
            * https://www.darkreading.com/application-security/attackers-have-been-leveraging-microsoft-zero-day-for-18-months
            * https://www.bleepingcomputer.com/news/security/windows-mshtml-zero-day-used-in-malware-attacks-for-over-a-year/
            * https://securityonline.info/check-point-research-details-0-day-flaw-cve-2024-38112-threatens-windows-users/
            * https://news.mynavi.jp/techplus/article/20240711-2983211/
        * CVE-2024-38080 Windows Hyper-V Elevation of Privilege Vulnerability
    * CVSS 9.x
        * CVE-2024-38074 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38076 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38077 Windows Remote Desktop Licensing Service Remote Code Execution Vulnerability
        * CVE-2024-38089 Microsoft Defender for IoT Elevation of Privilege Vulnerability
    * そのた
        * CVE-2024-38023 SharePoint RCE
            * PoCリリース
                * https://www.cvedetails.com/cve/CVE-2024-38023/?q=CVE-2024-38023
        * CVE-2024-38021 Microsoft Outlook ゼロクリックコード実行の可能性
            * https://securityonline.info/cve-2024-38021-zero-click-vulnerability-discovered-in-microsoft-outlook/
* KEV
    * CVE-2024-23692 Rejetto HTTP File Server Improper Neutralization of Special Elements Used in a Template Engine Vulnerability
    * CVE-2024-38080 Microsoft Windows Hyper-V Privilege Escalation Vulnerability
    * CVE-2024-38112 Microsoft Windows MSHTML Platform Spoofing Vulnerability
* regreSSHion (CVE-2024-6387) の各社アドバイザリ
    * https://securityonline.info/cisco-confirms-critical-openssh-regresshion-cve-2024-6387-flaw-in-multiple-products/
    * https://www.security-next.com/159425
    * https://fortiguard.fortinet.com/psirt/FG-IR-24-258
    * https://support.citrix.com/article/CTX678072/cloud-software-group-security-advisory-for-cve20246387
    * https://securityonline.info/cloud-software-group-confirms-cve-2024-6387-exposure-in-netscaler/

# その他
* Google ダークウェブレポート を無料開放
    * https://forest.watch.impress.co.jp/docs/news/1606361.html
* AppleStoreからいくつかのロシアのVPNアプリが削除される
    * https://www.bleepingcomputer.com/news/technology/russia-forces-apple-to-remove-dozens-of-vpn-apps-from-app-store/
    * https://thehackernews.com/2024/07/apple-removes-vpn-apps-from-russian-app.html
* Windows11 Notepad.exeにスペルチェックとオートコレクトが、すべてのユーザに実装
    * https://www.bleepingcomputer.com/news/microsoft/notepad-finally-gets-spellcheck-autocorrect-for-all-windows-11-users/
    * https://www.theregister.com/2024/07/08/it_only_took_41_years/
* Windows11 22H2 EOLが今年の10月
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-windows-11-22h2-reaches-end-of-service-in-october/
* Windows Update 7月。Windows Nエディションで不具合。配信一時停止中
    * https://www.bleepingcomputer.com/news/microsoft/microsoft-fixes-windows-11-bug-causing-reboot-loops-taskbar-freezes/
    * https://news.mynavi.jp/techplus/article/20240711-2983769/
* Google 高リスク向けユーザにパスキーを提供開始
    * https://thehackernews.com/2024/07/google-adds-passkeys-to-advanced.html
    * https://www.bleepingcomputer.com/news/security/google-advanced-protection-program-gets-passkeys-for-high-risk-users/
* Cloudflare、すべての生成AIによるクローラーをワンクリックでブロックする機能を無料で提供開始
    * https://www.publickey1.jp/blog/24/cloudflareai.html
    * https://blog.cloudflare.com/declaring-your-aindependence-block-ai-bots-scrapers-and-crawlers-with-a-single-click
* 新しいフィッシングツールキット FishXProxy
    * https://securityboulevard.com/2024/07/new-fishxproxy-phishing-kit-lowers-barriers-for-cybercriminals/
* 【第9回】情報セキュリティ事故対応アワード
    * https://news.mynavi.jp/techplus/article/20240711-2970146/
* JPCERT/CC インシデント相談・情報提供窓口対応状況
    * https://blogs.jpcert.or.jp/ja/2024/07/ir_consult.html
