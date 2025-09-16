---
title: "Offsec の CPE を 貯める"
emoji: "⚔️"
type: "tech"
topics: ["Offsec", "OSCP", "OSCP+", "OSTH", "OSIR", "OSCC", "SEC-100", "SJD-100", "ISC2", "CISSP"]
published: true
---

## 本記事について

- [Offsecは、継続学習ポイント(CPE) の制度を発表](https://www.webasha.com/blog/oscp-exam-update-what-is-oscp-certification?utm_source=chatgpt.com)し、[2025/04/08 から購入可能な形](https://help.offsec.com/hc/en-us/articles/31553032386964-OffSec-Continuing-Professional-Education-CPE-Program-Overview?#h_01JB17TXXCJTAZF5PXKG0RMR71) となった
- ISC2 資格保有者には馴染み深いCPE対応 について、集め方や注意点を確認しておく必要があるため、情報をとりまとめる
- 加えて、CISSP等のホルダーは、ISC2 / Offsec いずれもも対象となるCPEに関して集める形がより効率的な側面もあるので、それらの情報についてまとめる
- 何か追加があれば、PRかコメントをお待ちしております

# Offsec CPE プログラム について

- OffSecは、資格に「有効期限」が付くタイプの認定（例：OSCP+、OSTH、OSIR、OSCC等）を対象に、3年ごとの更新制度（certification renewal）の一環としてCPEプログラムを導入
- Annual Maintenance Fee (AMF) は、 1 年あたり US$145
    - 複数の対象資格を保有している場合も、1つのAMFでよい
- 更新方法は、以下の3つのいずれか
    - 3年サイクルで 120 CPEクレジット を取得すること
    - もう一度同じ資格に合格すること
    - 上位資格を獲得すること
- 詳細および最新の情報は、[OffSec CPE Program and Annual Maintenance Handbook](https://help.offsec.com/hc/en-us/articles/35366391096596-OffSec-CPE-Program-and-Annual-Maintenance-Handbook) を確認することを推奨

## AMFを支払うと受けられるもの
- 認定維持
- CPE関連コース(CPE-mapped content)
    - CPEを獲得できるEラーニングを受講できる

# 提出できる種類(と実績情報)

実際に提出を行い承認されたものも記録していく。  
公式の最新一覧は、[OffSec CPE Program and Annual Maintenance Handbook / CPE Content Pool](https://help.offsec.com/hc/en-us/articles/35366391096596-OffSec-CPE-Program-and-Annual-Maintenance-Handbook?#h_01JQY4CS5JYNG9R8TXXQ6W3N3A)  

- コースとセミナー (Courses and Seminars)
    - 未提出
- 公開講演 (Public Speaking)
    - 未提出
- 公開されたホワイトペーパー(Published White Papers)
    - 未提出
- OffSec ラボ提出物(OffSec Lab Submissions)
    - 未提出
- サイバーセキュリティ・ウェビナー参加(Attending Cybersecurity Webinars)
    - 未提出

# Offsecへ行った Q&A 

Offsecに質問を行った一覧。おそらく質問回答日時点の情報となるので、最新については、CPEハンドブックを確認推奨  

- Q: 資格取得年の、資格取得日以前のセキュリティ活動をCPE提出できますか？ 2025/08
    - No
- Q: Learn Unlimitedがある場合、AMFプランの購入が必要か？ 2025/08
    - No。Learn Unlimitedに含まれている
        - `Learn Unlimited already includes unlimited course access, unlimited exam attempts, and coverage for certification maintenance.`
    - Learn Unlimited を更新しない場合は、AMFの支払いが必要
- Q: Hardening Japan のような、日本で開催されるサイバーセキュリティイベントもCPE提出対象か？ 2025/09
    - 対象。申請には書類が必要
        - `Yes, you may submit relevant cybersecurity events such as conferences, seminars, or workshops, even those held in Japan, like Hardening JP. These fall under the Courses and Seminars category, which is eligible for CPE credit. Please be sure to include appropriate documentation (e.g., certificate of attendance or proof of participation) with your submission.`
- Q: CTFイベントは、CPE対象ですか？ 2025/09
    - No
- Q: CPE申請には、イベント認定書を添付する必要がありますか？ 2025/09
    - Yes, 外部CPEの提出には、イベント認定書が必要。フォームでは送れないので、追ってメールする形
        - `Yes, all external CPE submissions must be accompanied by supporting documentation. This may include a certificate of completion, proof of attendance, or other relevant materials. After submitting via the OffSec CPE Dashboard, please email the documentation along with your name and submission ID to challenges@offsec.com`
- Q: `ISC2ウェビナーを申請できますか？` 2025/09
    - 申請できる。1時間1CPE
        - `Yes, cybersecurity webinars, including those hosted by ISC², are considered valid CPE activities. You will receive 1 CPE per hour of attendance, provided you include proof of participation when submitting.`
- 確認中: OffsecのラボはCPE対象となるか、ISC2へ確認する
- 確認中: Learn Enterprise は、Learn Unlimited同様、AMFが含まれるか


# ISC2 のCPE との効率的な共存について

まず大前提として、いずれもAMFが発生する。こちらについては、いずれも支払う。  

CPE付与条件は、[ISC2 の CPEクレジット](https://japan.isc2.org/member_cpecredit.html) 記載の通りだが、OffsecのCPEクレジットの方が、より手を動かすものが多い印象。  
例えば、ISC2側には付与対象として掲載のある`Webinar、ポッドキャスト、プレゼンテーションの準備` や、`書籍、雑誌、ホワイトペーパーの購読` に関連するものがOffsecには、現状存在しないように感じられる。そのため、イベントや外部活動でもしっかりと申請していく必要がありそうと感じる。  
おそらく、OffsecのCPEを目標に活動をしていると、ISC2のCPEは満たすことが多い と、現状は感じる。  
注意点としては、ISC2は、グループA/B という保有資格への関連性が存在する。グループBであてられるCPEには限りがあるので、注意が必要。  

---

- 詳細および最新の情報は、公式情報である [OffSec CPE Program and Annual Maintenance Handbook](https://help.offsec.com/hc/en-us/articles/35366391096596-OffSec-CPE-Program-and-Annual-Maintenance-Handbook) を確認ください
- QAの内容については、最新でない可能性があるので、参考情報として活用ください
- 内容が最新ではないものがあれば、お気軽にコメントかPR、Xにて共有いただけると助かります
