# 시장 규모·투자·비즈니스 모델: 검증 반영 요약본

기준일 2026-11-14. 원 조사(market.research.json)에 이번 적대적 검증(실제 웹 검색 15회)을 반영했다. 이전 검증(market.verify.json)은 검색 없이 끝났으므로 그 판정은 버렸다. 표기 규칙: **벤더 주장**은 회사·CEO가 발표한 미감사 수치, **독립 평가**는 제3자 벤치마크·논문, **미확인**은 이번 검색으로 확인하지 못한 항목, **미확인(사전 지식)**은 검색 근거 없이 사전 지식에만 기댄 항목이다.

## 1. 영역 요약

- 탐지 전용 시장은 2025년 기준 약 7억~10억 달러로, 연 25~30% 성장이 전망된다. 판매용 시장조사 업체 추정치라 신뢰도는 낮다 ([Meticulous](https://www.meticulousresearch.com/product/deepfake-detection-market-6944), [SNS Insider](https://www.snsinsider.com/reports/deepfake-detection-market-11090)).
- 2024~2026년 자금은 기업용 실시간 통신·사칭 방어로 몰렸다. 순수 탐지 스타트업 한 곳의 조달액은 대개 1,000만~3,500만 달러다 ([TechCrunch-Modulate](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/)).
- 2026년에 통합이 시작됐다. Superhuman이 GPTZero를 인수했고(6월), Deel이 Clarity를 인수했으며(8월), KPMG가 Reality Defender 소수지분을 샀다(9월). 탐지는 단독 제품보다 플랫폼의 기능으로 흡수되는 추세다.
- 규모 있는 매출이 확인되는 곳은 Pindrop(음성, ARR 1억 달러 이상)과 텍스트 분야(GPTZero, Turnitin)뿐이다. B2C 범용 앱은 레드오션이다. 수사용 틈새도 국내에서는 국가 공동 시스템 계획 때문에 좁다.

## 2. 주요 제품 표 (중요도 순)

점수는 1~5. 신뢰도 점수는 벤더 주장만 있고 독립 평가가 없으면 원 조사보다 1점 낮췄다.

| 제품 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| Pindrop Pulse/Protect | Pindrop(미국) | 콜센터 플랫폼/API | 은행·보험·헬스케어 | 4 | 5 | 3 | 운영중 | 2025년 4월 ARR 1억 달러 돌파 공식 발표(회사 전체 기준, 벤더 주장) ([BiometricUpdate](https://www.biometricupdate.com/202504/pindrop-surpasses-100m-in-annual-recurring-revenue-kicks-off-bu-podcast)) |
| Turnitin AI 탐지 | Turnitin(미국) | 교육기관 번들 | 교육 | 5 | 5 | 2 | 운영중 | 2024년 매출 2.03억 달러는 Sacra 추정, AI 탐지 매출은 따로 공개되지 않음 ([Sacra](https://sacra.com/c/turnitin/)) |
| Reality Defender | Reality Defender(미국) | 플랫폼+API | 금융·정부·개발자 | 4 | 3 | 2 | 운영중, 2026년 9월 KPMG 소수지분 | 무료 50회/월, 유료 399달러/1,000회 공개 ([Intercom 가격](https://intercom.help/reality-defender/en/articles/12831411-managing-your-plan-billing)) |
| GPTZero | GPTZero → Superhuman(미국/캐나다) | 웹·API·기관 | 교육·소비자 | 3 | 5 | 2 | 2026년 6월 23일 인수 | 사용자 1,900만 명 이상, ARR 3,000만 달러(벤더 주장) ([CryptoBriefing](https://cryptobriefing.com/superhuman-acquires-gptzero-ai-detector/)) |
| YouTube Likeness Detection | Google(미국) | 플랫폼 내장 | 크리에이터 | 5 | 4 | 2 | 2026년 5월 모든 성인 크리에이터로 확대(실험 기능) | 무료, 음성 미지원 ([PetaPixel](https://petapixel.com/2026/05/18/youtube-will-help-you-find-videos-featuring-your-ai-clone/)) |
| Hive 딥페이크 탐지 | Hive(미국) | API·온프레미스 | 플랫폼·국방 | 4 | 3 | 3 | 운영중 | DoD DIU 2년 240만 달러 계약(조달 선정이며 성능 벤치마크는 아님) ([BusinessWire](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats)) |
| GetReal Protect/Inspect | GetReal(미국) | 실시간 보호+포렌식 | 기업·정부·언론 | 4 | 3 | 3 | 운영중 | Series A 1,750만 달러(In-Q-Tel 참여) ([SecurityWeek](https://www.securityweek.com/getreal-security-raises-17-5-million-to-tackle-gen-ai-threats/)) |
| Norton Genie / McAfee Deepfake Detector | Gen Digital/McAfee(미국) | 보안 번들 | 소비자 | 5 | 3 | 2 | 운영중 | 유료 보안 플랜과 OEM에 번들, 영어만 지원 ([SecurityBrief](https://securitybrief.co.uk/story/norton-rolls-out-ai-deepfake-scam-protection-for-intel-pcs)) |
| Doppel | Doppel(미국) | 사칭 대응 플랫폼 | Fortune 500 | 4 | 4 | 2 | 운영중 | Series C 7,000만 달러, 기업가치 6억 달러 이상(2025년 11월) ([SecurityWeek](https://www.securityweek.com/doppel-raises-70-million-at-600-million-valuation/)) |
| Modulate Velma Deepfake Detect | Modulate(미국) | 음성 API + AI 음악 탐지 | 기업 | 3 | 3 | 2 | 운영중(2026년 3월 출시) | 2026년 9월 2,500만 달러 조달, 누적 6,000만 달러 ([TechCrunch](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/)) |
| Resemble DETECT-3B Omni | Resemble AI(미국/캐나다) | API(생성+탐지) | 기업 | 3 | 3 | 2 | 운영중 | 정확도 98%와 리더보드 1위는 벤더 주장이고 Modulate가 같은 주장을 함 ([SiliconANGLE](https://siliconangle.com/2025/12/08/resemble-ai-hauls-13m-different-approach-deepfake-detection/)) |
| Clarity | Clarity → Deel(이스라엘/미국) | 화상면접 신원 검증 | HR | 3 | 2 | 2 | 2026년 8월 3일 인수 | 보도상 4,500만~5,000만 달러(현금+주식) ([TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/)) |
| Pangram | Pangram Labs(미국) | 웹·API | 교육·기업 | 3 | 3 | 3 | 운영중 | 2026년 7월 900만 달러 조달(Menlo) ([TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/)) |
| 딥브레인AI 탐지 | 딥브레인AI(한국) | API·수사기관 맞춤 | 경찰·기업 | 3 | 2 | 2 | 운영중 | TTA GS 1등급(품질 인증이며 정확도 벤치마크는 아님) ([유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366)) |
| Sensity AI | Sensity(네덜란드) | 플랫폼·포렌식 리포트 | KYC·수사·언론 | 2 | 2 | 2 | 운영중 | EIC Accelerator 총 €4.9M(보조금 €2.5M+지분) ([BiometricUpdate](https://www.biometricupdate.com/202607/sensity-ai-gets-eic-funding-for-forensics-focused-deepfake-detection-models)) |

표 밖 참고: Adaptive Security(시뮬레이션 교육, 탐지 제품 아님), Loti·Vermillio(초상·IP 관리), imper.ai(메타·행동 신호 기반, 2,800만 달러), Hiya(무료 음성 판별 Chrome 확장), TrueMedia(2025년 1월 폐쇄 후 오픈소스화, Georgetown이 이어받음), Neuramancer(€1.7M 프리시드).

## 3. 4개 기준 판정

**메이저성**: 범용 멀티모달 판별에서 지배적인 단일 브랜드는 없다. 영역별 강자가 나뉜다. 콜센터 음성은 Pindrop, 텍스트는 Turnitin과 GPTZero(현재 Superhuman), 소비자 접점은 빅테크·보안 번들(YouTube, Norton·McAfee)이다. 통합이 진행되면서 메이저 플랫폼 안의 기능이 되는 흐름이다 ([TNW-Deel](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection), [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html)).

**완성도·실사용**: 실사용 규모가 확인되는 곳은 텍스트(GPTZero 1,900만 명, 벤더 주장)와 콜센터 음성(Pindrop ARR 1억 달러, 벤더 주장)뿐이다. 멀티모달 스타트업은 매출이 공개되지 않았거나 작다(Sensity는 2026년 ARR 400만 달러 이상이 목표, 벤더 주장 ([Simplify](https://simplify.jobs/c/Sensity))). 소비자 앱스토어 탐지 앱은 비작동·사기성 리뷰가 많다 ([Copyleaks 블로그](https://copyleaks.com/blog/ai-detector-apps-arent-what-they-claim)).

**신뢰도**: 독립 평가인 Deepfake-Eval-2024에서 실제 유통 딥페이크에 대한 오픈소스 최신 탐지기 AUC가 기존 벤치마크 대비 영상 약 50%, 음성 48%, 이미지 45% 떨어졌다. 상용 모델도 포렌식 분석가 수준에는 못 미쳤다(2024년 유통물 기준) ([arXiv 2503.02857](https://arxiv.org/abs/2503.02857)). 경찰청 탐지 SW의 탐지율도 약 80%여서 수사 방향 설정용으로만 쓴다 ([보안뉴스](https://m.boannews.com/html/detail.html?idx=127364)). 벤더 정확도(Resemble 98%, Modulate 98.9%/EER 1.1%, Hiya 99%, Pangram 1/10,000 오분류)와 리더보드 1위 주장은 모두 벤더 주장이다.

**신규 진입 경쟁력(개인·소규모 팀)**: 낮음~제한적. B2C 범용 앱은 무료 대체재 때문에 수익화가 어렵다. 기업 실시간 방어는 자본 격차가 크다. Reality Defender가 공개 가격(약 0.4달러/스캔, 무료 50회)을 내놓아 저가 API의 가격 상한선을 정한다. 국내 수사용은 경찰청이 수사기관 공동 시스템을 계획하고 있어 좁다. 남는 여지는 보험·법무·언론용 감정 리포트와 채용 같은 좁은 버티컬이고, 엑시트는 플랫폼 인수형이 현실적이다.

## 4. 레드오션 판정: **부분적**

- **B2C 범용 판별 앱: 예.** YouTube, Google SynthID, Hiya, Norton·McAfee, Reality Defender 무료 티어 같은 무료·번들 대체재가 있다 ([SocialMediaToday](https://www.socialmediatoday.com/news/youtube-expands-likeness-detection-to-all-users-over-18/820440/), [SSN](https://www.securitysystemsnews.com/article/reality-defender-launches-public-api-and-free-tier)). 앱스토어 앱은 평판이 나쁘고, 무료 비영리 TrueMedia는 독자 운영을 접었다 ([TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia)).
- **기업 실시간 사칭 방어: 예(자본 집약 경쟁).** Pindrop, Reality Defender, GetReal, Doppel, Modulate, imper.ai가 수천만~억 달러를 확보했다.
- **포렌식·수사용 고신뢰 판별: 기술적으로는 미해결이지만 시장은 좁다.** 원 조사의 '아직 기회'라는 판단은 국내 기준으로 과대평가다. 경찰청은 R&D(91억 원)가 끝나면 모든 수사기관이 공동으로 쓰는 시스템을 구축할 계획이고, 2026년 8월에는 탐지 SW, AI 전문분석관, 범행도구 분석의 '3중 대응'을 발표했다 ([korea.kr](https://www.korea.kr/news/policyNewsView.do?newsId=148973649), [뉴데일리](https://www.newdaily.co.kr/site/data/html/2026/08/13/2026081300088.html)). 해외에도 GetReal Inspect와 Sensity가 있다.
- **특허**: 탐지 모델 자체에 대한 소송은 찾지 못했다. 다만 C2PA·출처 검증 영역에는 KeeeX의 UPC 소송 신호가 있다(6절).

## 5. 빈틈·기회

- **비수사기관용 포렌식 감정 리포트(보험·법무·언론)**: 재현 가능한 분석, 근거 제시, chain of custody를 갖춘 제품은 적다. Coalition이 딥페이크 대응 특약에 포렌식 분석과 서면 보고서를 넣었다 ([Reinsurance News](https://www.reinsurancene.ws/coalition-enhances-cyber-product-with-addition-of-deepfake-response-endorsement)). (원 조사가 근거로 든 'Sensity NIST CFTT 등재'는 확인되지 않아 뺐다.)
- **한국어·국내 플랫폼 특화**: Norton 기능은 영어만 지원한다 ([SecurityBrief](https://securitybrief.co.uk/story/norton-adds-ai-powered-deepfake-detection-to-genie-assistant)). 수요처는 보이스피싱 대응 금융권, 언론, 법무다. 수사기관 조달은 국가 시스템과 경쟁하게 된다.
- **채용 사기 플러그인**: Gartner는 2028년 지원자 프로필 4개 중 1개가 가짜일 수 있다고 전망했다(전망치) ([Allwork](https://allwork.space/2025/04/ai-deepfake-scammers-infiltrating-the-hiring-processes-at-alarming-rates-gartner-reports/)). Deel의 Clarity 인수가 이 수요를 겨냥했다. 엑시트는 인수형이다.
- **탐지와 출처 검증(C2PA·SynthID)을 합친 종합 리포트**: 탐지만으로는 한계가 있다 ([arXiv](https://arxiv.org/abs/2503.02857)). 단, KeeeX 특허 소송 리스크를 점검해야 한다.
- **AI 음악 판별**: 원 조사는 빈틈으로 봤으나, Modulate가 AI 음악 탐지 도구를 이미 운영 중이어서 기회가 줄었다 ([MBW](https://www.musicbusinessworldwide.com/audio-ai-firm-modulate-which-runs-an-ai-music-detection-tool-raises-25m/)).
- **중소 금융용 저가 API**: Reality Defender 공개 가격(399달러/1,000회)이 기준선이다. IDV 벤더(Persona, Jumio, iProov)가 이미 이 자리를 차지하고 있다는 지적은 미확인(사전 지식).

## 6. 위협·장벽

- **무료 대체재**: YouTube Likeness Detection(무료, 실험 기능, 일부 국가) ([The Decoder](https://the-decoder.com/youtube-opens-its-deepfake-face-swap-detection-tool-to-all-adult-creators/)), Hiya 확장 ([Engadget](https://www.engadget.com/ai/a-new-chrome-extension-can-reliably-detect-ai-generated-voices-130059842.html)), Reality Defender 무료 티어. ElevenLabs 분류기, Intel FakeCatcher 같은 생성사·칩사 탐지기는 미확인(사전 지식).
- **가격 기준선**: 엔터프라이즈 탐지 API 공개가는 약 0.4달러/스캔이다 ([Toolradar](https://toolradar.com/tools/reality-defender/pricing)).
- **자본 격차**: Pindrop 지분 투자 2.183억 달러에 부채 1억 달러 ([HelpNetSecurity](https://www.helpnetsecurity.com/2024/07/18/pindrop-financing-100-million/)), Doppel 누적 약 1.24억~1.29억 달러, Adaptive Series B 8,100만 달러 ([BankInfoSecurity](https://www.bankinfosecurity.com/adaptive-security-gets-81m-series-b-for-ai-deepfake-defense-a-30332)), Modulate 누적 6,000만 달러.
- **B2G 대체 리스크**: 경찰청 국가 R&D 91억 원(숭실대 컨소시엄, 한컴위드 참여, 부퍼탈대 공동연구)이 끝나면 수사기관 공동 시스템이 생긴다 ([디지털데일리](https://www.ddaily.co.kr/page/view/2025020211334778803), [바이라인](https://byline.network/2025/06/5-299/)). GS 인증 같은 조달 요건도 있다.
- **정확도와 법적 책임**: 실제 유통물에서 성능이 크게 떨어지고, 새 생성 모델이 나올 때마다 다시 떨어진다. 수사급 신뢰도를 주장하면 오탐·미탐에 대한 책임 위험이 크다.
- **특허**: KeeeX SAS(프랑스 NPE)가 EP2949070(데이터 블록 무결성 검증)을 근거로 OpenAI, Adobe, Truepic, C2PA를 UPC에 제소했다는 보도가 있다. 2025년, 2차 출처이고 현황은 미확인 ([Substack](https://michael7924.substack.com/p/openaiadobe-and-truepic-sued-by-a)). 탐지 모델 자체에 대한 2025~2026년 소송은 찾지 못했다. Pindrop 등의 특허 보유 현황은 미확인.
- **엑시트 구조**: 대부분 플랫폼 인수형이다. Clarity 대금은 현금과 주식이 섞여 있어 '누적 투자의 약 3배'를 현금 회수로 읽으면 과장이다.
- **인식과 지출의 격차**: 보안 리더의 약 3/4이 딥페이크 공격을 겪었거나 의심했지만, 전용 방어책을 갖춘 곳은 10%다(벤더 조사) ([HelpNetSecurity](https://helpnetsecurity.com/2026/09/29/pindrop-enterprise-deepfake-attacks-report)). Coalition은 청구 건의 98%가 고급 AI와 무관하다고 밝혔다 ([CyberScoop](https://cyberscoop.com/?p=87093)).
- **규제(EU AI Act 제50조, 한국 AI 기본법)**: 시행일은 미확인(사전 지식). 표시 의무가 출처 검증 수요를 만든다.

## 7. 핵심 사실 목록

- 시장 규모(탐지 전용, 판매용 추정치): Meticulous는 2025년 7.1억 달러, 2026년 9.9억 달러, 2036년 94.4억 달러(CAGR 25.3%)로 본다 ([Meticulous](https://www.meticulousresearch.com/product/deepfake-detection-market-6944)). SNS Insider는 2025년 9.19억 달러에서 2035년 121억 달러 ([SNS Insider](https://www.snsinsider.com/reports/deepfake-detection-market-11090)), Astute Analytica는 2025년 7.0억 달러에서 2035년 90억 달러로 본다 ([Astute](https://www.astuteanalytica.com/industry-report/deepfake-detection-market)). LP Information(2024년 1.98억 달러)과 MRFR(2024년 17.32억 달러)은 이상치이거나 정의가 다르며 재확인하지 못했다(미확인).
- 피해 전망: Deloitte는 미국 생성형 AI 사기 손실을 2023년 123억 달러에서 2027년 400억 달러로 본다(시나리오 전망) ([Deloitte](https://www.deloitte.com/us/en/insights/industry/financial-services/deepfake-banking-fraud-risk-on-the-rise.html)). Resemble의 2025년 피해 12.8억 달러 이상은 벤더 집계이고 내부 수치끼리 맞지 않는다 ([Resemble](https://resemble.ai/2025-deepfake-threat-report)).
- GPTZero: 2026년 6월 23일 Superhuman이 인수했다. 조건은 비공개이고 8,800만 달러 이상은 매체 추정이다. 사용자 1,900만 명 이상(한 매체는 2,000만 명 이상), ARR 3,000만 달러는 벤더 주장이다. 누적 투자는 1,350만 달러다 ([AI Weekly](https://aiweekly.co/alerts/superhuman-acquires-gptzero-to-add-ai-authenticity-layer), [TechCrunch](https://techcrunch.com/?p=3135465)).
- Clarity: 2026년 8월 3일 Deel이 인수했다. Deel의 15번째 인수이자 첫 이스라엘 기업 인수이며, 보도상 4,500만~5,000만 달러를 현금과 주식으로 지급했다(Calcalist는 4,000만~5,000만 달러). 2024년 시드는 1,600만 달러였다 ([Calcalist](https://calcalistech.com/ctechnews/article/bkeyex0sgl), [Dealroom](https://dealroom.co/news/142736-deel-acquires-clarity-to-strengthen-identity-verification-surpasses-1-5b/)).
- KPMG: 2026년 9월 10일 Reality Defender 소수지분을 인수했다(조건 비공개) ([KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html), [IAB](https://www.internationalaccountingbulletin.com/news/kpmg-llp-acquires-stake-in-deepfake-detection-business-reality-defender/)). Reality Defender의 Series A는 3,300만 달러다 ([DCVC](https://dcvc.com/press-releases/reality-defender-expands-series-a-to-33-million-to-enhance-ai-detection-capabilities)).
- Pindrop: 2025년 4월 ARR 1억 달러를 넘었다고 공식 발표했다. CEO는 매출이 1억 달러를 '훨씬 넘고' 2025년부터 현금흐름 흑자이며 직원이 300명 이상이라고 말했다(벤더 주장) ([Mergermarket](https://ionanalytics.com/insights/mergermarket/pindrop-could-step-up-acquisitions-in-agentic-security-as-its-deepfake-detection-takes-off-ceo/)).
- Doppel: 2025년 11월 19일 Series C 7,000만 달러를 조달했다(Bessemer 주도). 기업가치는 2025년 5월 약 2.05억 달러에서 6억 달러 이상으로 올랐다 ([Doppel 보도자료](https://www.doppel.com/company/press-releases/doppel-raises-series-c-to-meet-rising-demand-for-ai-driven-social-engineering-defense)).
- Modulate: 2026년 9월 2,500만 달러를 조달했다(Future Ventures 주도, 누적 6,000만 달러, 직전 기업가치 1.7억 달러). 월 1,000만 시간 이상 오디오를 처리한다고 주장한다(벤더 주장) ([SiliconANGLE](https://siliconangle.com/2026/09/28/voice-ai-startup-modulate-raises-25m-to-bring-audio-native-models-to-more-developers/)).
- 기타 투자: GetReal 1,750만 달러, imper.ai 2,800만 달러 ([SecurityWeek](https://www.securityweek.com/imper-ai-emerges-from-stealth-mode-with-28-million-in-funding/)), Loti 1,620만 달러 ([BusinessWire](https://www.businesswire.com/news/home/20250415846205/en)), Vermillio 1,600만 달러 ([Axios](https://www.axios.com/2025/03/03/vermillio-ai-rights-licensing-sony-music)), Resemble 1,300만 달러, Pangram 900만 달러, Neuramancer €1.7M ([Tech.eu](https://tech.eu/2026/03/12/neuramancer-lands-eur17m-pre-seed-to-scale-deepfake-detection-tools)). Allure Security의 1,700만 달러 Series B는 미확인.
- 경찰청: 탐지 SW는 한국인 관련 인물 5,400명의 데이터 520만 점으로 학습했고 탐지율은 약 80%다 ([보안뉴스](https://m.boannews.com/html/detail.html?idx=127364)). 2024년 11월부터 1년간 딥페이크 범죄 1,553건을 집계했고, 2026년 1~7월 피의자 419명을 검거했다 ([보안뉴스](https://m.boannews.com/html/detail.html?idx=134010), [뉴데일리](https://www.newdaily.co.kr/site/data/html/2026/08/13/2026081300088.html)).
- YouTube Likeness Detection: 2025년 10월 YPP 대상으로 출시돼 2026년 5월 만 18세 이상 모든 크리에이터로 확대됐다. 신분증과 셀피 인증이 필요하고 음성은 지원하지 않는다 ([MacRumors](https://www.macrumors.com/2025/10/21/youtube-ai-likeness-detection-tool/)).

## 8. 검증에서 정정·삭제된 주요 사항

- **삭제**: 경찰 탐지 SW '누적 1,636건 수사 활용'은 확인되지 않아 근거에서 뺐다. 확인된 수치는 1,553건(집중단속 기간 범죄 집계)과 419명 검거다.
- **삭제**: Sensity 'NIST CFTT 카탈로그 등재'는 확인되지 않았다. 이에 따라 Sensity 신뢰도를 3에서 2로 낮췄다.
- **정정**: 시장 규모의 '약 10배 편차'는 정의가 다른 보고서를 섞은 결과였다. 탐지 전용 기준으로는 2025년 약 7억~10억 달러, 연 25~30% 성장으로 모인다.
- **정정**: Reality Defender에는 맞춤형 플랜만 있는 것이 아니다. 공개 유료 티어(월 399달러, 1,000회)가 있고, 무료 사용자는 소셜 링크 분석을 쓸 수 없다.
- **정정**: Resemble의 'Hugging Face 1위'는 Modulate의 같은 주장과 충돌하는 벤더 마케팅이다. 신뢰도를 3에서 2로 낮췄다.
- **정정**: Sensity EIC 금액은 €4.9M이다(€2.5M 보조금과 지분 투자).
- **정정**: Clarity 금액은 4,500만~5,000만 달러이고 주식이 섞여 있다. '약 3배 엑시트'를 현금 회수로 읽으면 과장이다.
- **정정**: GPTZero의 8,800만 달러는 공식 금액이 아니라 매체 추정이다.
- **정정**: 특허는 '완전 미확인'이 아니다. C2PA 관련 KeeeX UPC 소송이라는 신호가 있다.
- **추가(missed)**: Modulate(음성·AI 음악 탐지), Pindrop의 ARR 공식 발표, 경찰청의 수사기관 공동 시스템 계획과 3중 대응, Reality Defender 공개 가격, Neuramancer 등 신규 진입자.
- **판단 하향**: '포렌식·수사용은 아직 기회'라는 원 조사 결론은 국내 기준으로 과대평가였다. B2G 대체 리스크를 반영했다. '음악 판별 빈틈'도 Modulate 때문에 축소했다.
- **점수 조정**: 벤더 주장만 있는 항목의 신뢰도를 1점 낮췄다(Reality Defender, GPTZero, YouTube, Resemble, 딥브레인AI, Sensity). Pindrop 실사용은 공식 ARR 발표를 근거로 5를 유지했다.
- **여전히 미확인**: Adaptive 누적 1.465억 달러(Series B 8,100만 달러는 확인), AI or Not 등 소비자 앱의 재무, Arup 사건과 FBI IC3 통계, 규제 시행일.
