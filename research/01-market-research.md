# AI 생성물 판별 앱 시장조사 보고서

조사 시점: 2026-11-14 · 대상: 영상·사진·음성·음악·글의 AI 생성 여부 판별

## 0. 결론 요약

**한 줄 결론: "영상·사진·음악·글을 넣으면 AI인지 알려 주는 범용 소비자 앱"은 레드오션이고, "범죄까지 잡는 정교한 모델"은 빅테크와 정부도 아직 못 만든 목표다. 범용 앱이라면 포기가 맞다. 다만 특허가 막고 있지는 않으므로, 좁은 B2B 영역(민간 분쟁용 설명형 감정 리포트 등)으로 방향을 바꾼다면 조건부로 해 볼 만하다.**

### 0.1 질문별 직답

| 질문 | 답 | 핵심 근거 |
|---|---|---|
| ① 시장에 이미 있나? | **있다. 많다.** | 모달리티마다 제품 수십 개. 영상 [Reality Defender](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html), 음성 [Pindrop](https://www.biometricupdate.com/202504/pindrop-surpasses-100m-in-annual-recurring-revenue-kicks-off-bu-podcast), 음악 [Deezer](https://dataconomy.com/2026/01/29/music-streaming-giant-deezer-opens-ai-detection-tool-to-external-platforms/), 글 [GPTZero](https://www.businesswire.com/news/home/20260623083788/en/Superhuman-to-Acquire-GPTZero-AI-Authenticity-Platform) (2절) |
| ② 메이저한 앱이 있나? | **모달리티별로는 있다. 네 매체를 다 하는 메이저 소비자 앱은 없다.** | Google SynthID Detector는 무료지만 글 제외, 워터마크 확인만 [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/). 가장 비슷한 Bitdefender RealCheck는 영상 중심·영어 전용 [Bitdefender](https://www.bitdefender.com/en-us/news/bitdefender-launches-realcheck-a-powerful-deepfake-detection-solution) |
| ③ 완성도가 높고 많이 쓰이나? | **B2B와 글은 많이 쓴다. 소비자 판별 앱은 거의 안 쓴다.** | 미국 교사 68%가 글 탐지기 정기 사용 [CDT](https://cdt.org/insights/new-research-educators-still-struggling-with-generative-ai-detection-discipline-and-distrust-despite-increased-school-guidance/). 이미지 판별 전용 앱 중 설치 10만 건 넘는 앱은 못 찾음 [AppBrain](https://www.appbrain.com/dev/Zyur/) |
| ④ 믿을 만한가? | **아니다(범죄 판단 기준).** 벤더는 95~99%를 주장하지만 독립 평가는 훨씬 낮다. | 실제 유통 딥페이크에서 오픈소스 탐지기 AUC가 영상 50%·음성 48%·이미지 45% 하락, 상용도 사람 분석가 미달(독립 평가) [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857). 최신 이미지 생성기 탐지율 18~30%(독립 평가) [arXiv 2602.07814](https://arxiv.org/html/2602.07814) |
| ⑤ 레드오션인가? | **범용은 예. 일부 니치는 아직 아니지만 좁아지는 중.** | 이미지·영상·음성 = 부분적, 음악 = 예, 영어 글 = 예, 통합 소비자 앱 = 예(수익 관점). 2026년 인수·통합 시작 [TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/) |
| ⑥ 특허로 막혔나? | **아니다. 다만 구현 특허는 쌓이는 중.** | 개념 전체를 막는 특허는 발견 안 됨. C2PA(KeeeX 소송)·얼굴 라이브니스(FaceTec)는 고위험 [JUVE Patent](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/) [Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents). 법률 자문 아님, FTO 필요 |
| ⑦ 지금 만들어도 경쟁력이 있나? | **범용 소비자 앱은 없다. 좁은 B2B 니치는 조건부로 있다.** | 빅테크 무료 확인 기능 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/), 한국 수사·선거는 정부 자체 개발 [다음](https://v.daum.net/v/6VGDUSx2ab), 실시간 통화 탐지는 삼성·통신사 무료 [바이라인](https://byline.network/2026/02/12-535/) |

### 0.2 최종 권고: 조건부 진행

원래 구상(범용 소비자 앱 + 범죄 수준 판별)은 **포기**를 권한다. 사용자가 정한 포기 기준("레드오션이면 포기") 중 레드오션 조건에 해당하기 때문이다. 특허 조건에는 해당하지 않는다.

대신 방향을 바꾼다면 **조건부 진행**이 가능하다. 아래 조건을 모두 받아들일 수 있을 때만 진행하라.

1. **소비자 앱이 아니라 좁은 B2B로 간다.** 첫 타깃은 로펌·보험사·노무·언론처럼 "근거가 있는 판단"에 돈을 내는 곳이다. 앱은 인지도·데이터를 모으는 입구로만 쓴다 (8절).
2. **"AI 확률 점수"가 아니라 설명형 리포트를 판다.** 메타데이터·편집 흔적·워터마크/C2PA 확인·탐지 결과를 한 장에 묶고, "진짜 / 가짜 / 판정 불가" 3단으로 답한다. 수사 현장도 AI 판별을 1차 선별로만 쓴다 [Amped](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165).
3. **오류율을 공개하고 독립 검증을 받는다.** 국산 제품 중 독립 벤치마크로 검증된 것이 하나도 없다는 점이 오히려 차별점이 된다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364).
4. **상업 이용 가능한 데이터만 쓴다.** GenImage·FaceForensics++·DeepfakeBench는 상업 이용 금지다 [GenImage](https://genimage-dataset.github.io). 실제 성착취 딥페이크는 소지만으로 처벌되므로 학습용으로 모을 수 없다 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877).
5. **출시 전 변리사 FTO를 받고, C2PA 서명·eKYC 라이브니스로는 확장하지 않는다.** 이 두 영역에서 실제 특허 분쟁이 진행 중이다 (6절).

이 조건이 싫다면, 즉 "누구나 쓰는 범용 판별 앱"이 아니면 의미가 없다면 **포기하는 것이 근거에 맞는 판단**이다.


## 1. 조사 방법·기준·한계

### 1.1 조사 시점과 범위

- **조사 시점:** 2026-11-14 기준. 이후 출시·인수·법 개정은 반영하지 않았다.
- **9개 조사 영역:** 이미지, 영상, 음성, 글(텍스트), 출처증명·워터마크(C2PA·SynthID), 한국 시장, 신뢰도(독립 평가·포렌식), 특허·데이터 라이선스, 시장 규모·투자. 음악은 음성 영역에서 함께 조사했다.
- **가정:** 사용자는 개인 또는 소규모 초기 팀이다.

### 1.2 조사 과정

| 단계 | 한 일 |
|---|---|
| 1. 조사 | 영역별로 웹 자료(기사, 회사 발표, 논문, 정부 자료)를 모아 제품·수치·출처를 표로 정리 |
| 2. 적대적 검증 | 영역마다 실제 웹 검색(약 15회)으로 다른 검토자가 각 주장을 반박하는 입장에서 다시 확인. 출처가 약하거나 재확인 안 된 수치는 "미확인"으로 내리거나 삭제 |
| 3. 요약 | 검증을 통과한 내용만 영역별 요약본으로 압축. 이 보고서는 요약본에 근거한 내용만 쓴다 |

### 1.3 평가 기준과 점수

사용자가 준 네 기준을 그대로 썼다. 2절 표의 점수는 1~5점이다.

| 기준 | 묻는 것 | 1점 | 3점 | 5점 |
|---|---|---|---|---|
| 메이저성 | 누가 만들었고 얼마나 알려졌나 | 개인·무명 개발자 | 전문 스타트업·업계에서 알려짐 | 빅테크·대형 보안사·시장 표준 |
| 실사용(완성도) | 실제로 얼마나 쓰이나 | 거의 안 쓰임·중단 | 특정 고객군에서 운영 중 | 수천만 명 또는 기본 탑재 |
| 신뢰도 | 판정을 믿을 수 있나 | 근거 없음·잘 틀림 | 벤더 주장만 있거나 제한적 검증 | 독립 평가에서 실전 성능 확인 |
| 경쟁력(신규 진입) | 지금 소규모 팀이 들어가 이길 수 있나 | 무료 대체재·대기업 점유 | 니치에 틈 있음 | 비어 있고 수요 확인 |

"레드오션"은 **예 / 부분적 / 아니오**로 판정했다. 무료 대체재, 대형 사업자의 유통 장악, 인수·통합 여부를 함께 봤다.

### 1.4 근거를 다루는 원칙

- **"벤더 주장"과 "독립 평가"를 구분한다.** 회사가 스스로 발표한 정확도(대개 95~99%)는 "벤더 주장", 제3자 논문·언론 테스트는 "독립 평가"로 표시했다. 둘이 다르면 독립 평가를 더 무겁게 본다.
- 정부 발표도 독립 평가가 아니다. 국과수·경찰청 수치는 "정부 발표"로 표시했다.
- GS인증은 소프트웨어 품질 인증이지 탐지 정확도 검증이 아니다.
- 요약본끼리 수치가 엇갈리면 출처가 더 확실한 쪽을 쓰고, 엇갈린다는 사실을 본문에 짧게 적었다(예: 국과수 정확도 92% vs 97%).

### 1.5 한계

- **웹 검색 한도:** 적대적 검증은 영역마다 웹 검색 약 15회로 제한됐다. 그래서 일부 항목은 재확인하지 못하고 **"미확인"**으로 남았다. 조사자의 사전 지식에만 기댄 내용은 **"미확인(사전 지식)"**으로 표시했다.
- **특허:** 청구항 전문을 원문으로 확인하지 못했고 서지 사항만 확인했다. 미국 법원 기록(PACER)은 조회하지 않았다. 이 보고서는 법률 자문이 아니다.
- **시장 규모:** 판매용 조사 보고서의 추정치라 신뢰도가 낮다.
- **앱 사용자 수:** 대부분의 회사가 공개하지 않아 다운로드 수·자기 진술로 추정했다.
- **표본:** 언론 테스트(NewsGuard 30장, EDMO 15장 등)는 표본이 작다.


## 2. 모달리티별 현황

> 읽는 법: 점수는 1~5(5가 가장 높음). "벤더 주장"은 회사가 스스로 발표한 수치, "독립 평가"는 제3자 논문·언론 테스트 결과다. 같은 제품이라도 모달리티마다 점수가 다를 수 있다.

### 2.1 이미지

| 제품 | 회사 | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| SynthID Detector·Gemini 검증 | Google(미국) | 웹·Gemini·Chrome | 소비자·언론 | 5 | 5 | 3 | 무료. Google 등 워터마크 있는 것만 판별, "범용 탐지기 아님" [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/) |
| Hive AI 탐지 | Hive(미국) | API·크롬 확장 | 플랫폼·정부 | 5 | 4 | 3~4 | 독립 평가 98.03%(구형·교란 없는 AI 아트) [arXiv 2402.03214](https://arxiv.org/pdf/2402.03214), 미 국방부 240만 달러 계약 [BusinessWire](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats) |
| Amped Authenticate | Amped Software(이탈리아) | 포렌식 SW | 수사기관 | 4 | 4 | 3 | 벤더 스스로 "증거가 아니라 선별용" [Amped](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165) |
| Magnet Verify/Axiom | Magnet Forensics(캐나다) | 포렌식 플랫폼 | 수사·검찰 | 4 | 4 | 3 | "법정 방어 가능" 표방(벤더 주장) [Magnet](https://www.magnetforensics.com/blog/authenticity-on-trial-how-magnet-verify-helps-prosecutors-admit-digital-media-and-defeat-deepfake-defenses/) |
| Reality Defender | Reality Defender(미국) | 플랫폼·API | 금융·정부 | 4 | 3 | 3 | 무료 월 50건, 월 399달러/1,000건. 이미지 독립 평가 없음 [RD API](https://realitydefender.com/api) |
| OpenAI Verify | OpenAI(미국) | 웹(프리뷰) | 소비자 | 5 | 3 | 3 | OpenAI 출처 신호만 확인 [OpenAI](https://help.openai.com/en/articles/8912793-provenance-signals-content-credentials-synthid-in-openai-generated-content) |
| Adobe Content Authenticity | Adobe(미국) | 무료 웹·확장 | 크리에이터 | 5 | 3 | 3 | C2PA 판독 전용, 메타데이터 지우면 불가 [arXiv 2604.24890](https://arxiv.org/pdf/2604.24890) |
| AI or Not | AI or Not(미국) | 웹·API | 소비자·KYC | 3 | 3 | 3 | 98.9%(벤더 주장). 사용자 수는 자기 진술뿐 [DataInnovation](https://datainnovation.org/2025/08/5-qs-with-anatoly-kvitnitsky-ceo-of-ai-or-not/) |
| Sightengine | Sightengine(프랑스) | API | 개발자 | 3 | 3 | 3 | 월 29달러부터 [Sightengine 가격](https://sightengine.com/pricing) |
| GetReal Inspect | GetReal(미국) | 엔터프라이즈 | 보안·정부 | 4 | 3 | 3 | 성능 비공개, 1,750만 달러 투자 [GetReal](https://www.getrealsecurity.com/resources/getreal-security-raises-17-5m-series-a-led-by-forgepoint-capital-to-address-rapidly-growing-threats-associated-with-generative-ai-and-malicious-digital-media) |
| 딥브레인AI AI 디텍터 | 딥브레인AI(한국) | SaaS·API | 수사·공공 | 3 | 3 | 3 | 경찰청 SW 1차 개발 협력(경찰청 SW 누적 1,636건 활용, 4.4 참고). 90% 이상은 벤더 주장 [뉴스핌](https://www.newspim.com/news/view/20260813000619) |
| Pangram Image | Pangram(미국) | 웹·API | 기업·교육 | 3 | 2 | 2 | 연구 프리뷰, 99.5%는 벤더 주장 [TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/) |
| ForgeSpy(소비자 앱 예) | Zyur(미확인) | 모바일 앱 | 소비자 | 1 | 2 | 2 | 약 1.76만 설치(추정) [AppGoblin](https://appgoblin.info/apps/io.zyur.forgespy) |

Amped·Magnet의 본사 국가는 요약본에 별도 출처 없이 적힌 값이다.

**4개 기준 판정**
- **메이저성: 있음.** Google·OpenAI·Adobe가 무료 검증을 기본 기능으로 넣었다. 다만 이들은 자사·파트너 워터마크 확인기이고 범용 탐지기가 아니다. Midjourney는 워터마크를 넣지 않는다(2차 출처) [c2paviewer](https://c2paviewer.com/articles/ai-tools-c2pa-support).
- **완성도·실사용: 소비자 앱은 낮음.** 설치 10만 건이 넘는 이미지 판별 전용 앱은 찾지 못했다 [AppBrain](https://www.appbrain.com/dev/Zyur/). 수사 현장에서는 Amped·Magnet이 이미 쓰인다 [ForensicFocus](https://www.forensicfocus.com/news/advanced-detection-tools-from-amped-software-aim-to-combat-ai-generated-csam-and-protect-children/).
- **신뢰도: 범죄 수사 기준으로는 낮음.** 독립 평가에서 오픈소스 16종의 최고 평균 정확도는 75%, 최신 생성기(Midjourney v7·Flux 등) 탐지율은 18~30%였다 [arXiv 2602.07814](https://arxiv.org/html/2602.07814). 실제 사진 15장 테스트에서 평균 오탐 13.3%(독립 평가, 표본 작음) [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/). 워터마크도 제거 공격(SynthID-Image 100% 제거)에 뚫렸다 [arXiv 2608.10166](https://arxiv.org/pdf/2608.10166).
- **신규 진입 경쟁력: 범용은 낮고 니치는 조건부.** 무료 대체재와 자금 격차(Hive 2021년 기업가치 20억 달러 [SiliconANGLE](https://siliconangle.com/2021/04/21/enterprise-ai-solutions-startup-hive-raises-85m-2b-valuation/))가 크다. 반면 "학습 데이터가 구조보다 중요"하다는 결과는 한국·문서 위조 같은 특화 데이터에 유리하다 [arXiv 2602.07814](https://arxiv.org/html/2602.07814).

**레드오션 판정: 부분적**
- 범용 소비자 판별 앱은 **예**. 저품질 앱 난립, 빅테크 무료 검증, 도구별 오탐 0~40%로 신뢰 형성이 어렵다 [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/).
- 수사·포렌식도 블루오션이 아니다. Amped·Magnet이 조달 채널과 법정 실적을 쥐고 있다. 남은 틈은 부분 합성 위치 표시, 문서·신분증 위조, 한국 특화 데이터다 [HF 2606.19259](https://huggingface.co/papers/2606.19259.md).
- 특허는 장벽이 아니다. C2PA 관련 KeeeX 소송은 원고에게 불리하게 진행 중이다 [UPC 명령](https://www.unifiedpatentcourt.org/sites/default/files/files/api_order/922-2026%20Adobe%20ea%20Final%20Order%20en-GB.pdf).

### 2.2 영상·딥페이크

| 제품 | 회사 | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| Reality Defender | Reality Defender(미국) | 플랫폼·API·회의 탐지 | 기업·정부 | 4 | 3 | 3 | Gartner 선정, KPMG 소수지분 투자. 독립 벤치마크 없음 [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html) |
| GetReal Security | GetReal(미국) | 포렌식·신원 | 기업·정부 | 4 | 3 | 3 | 성능 비공개 [SecurityWeek](https://www.securityweek.com/getreal-security-raises-17-5-million-to-tackle-gen-ai-threats/) |
| Pindrop Pulse for Meetings | Pindrop(미국) | 회의 실시간 탐지 | 기업 | 4 | 4 | 3 | Zoom·Teams·Webex 지원, 음성이 주력 [BusinessWire](https://www.businesswire.com/news/home/20251119488893/en) |
| Hive | Hive(미국) | API·크롬 확장 | 플랫폼·국방 | 4 | 4 | 3 | 확장 사용자 약 5만 명 [Chrome 웹스토어](https://chromewebstore.google.com/detail/hive-ai-detector/cmeikcgfecnhojcbfapbmpbjgllklcbi?hl=fil) |
| Bitdefender RealCheck | Bitdefender(루마니아) | 모바일 독립 앱 | 소비자 | 4 | 2 | 2 | 구상 앱과 가장 비슷. 영어 전용, 월 4.99달러, 성능 비공개 [Bitdefender](https://www.bitdefender.com/en-us/news/bitdefender-launches-realcheck-a-powerful-deepfake-detection-solution) |
| McAfee Deepfake Detector | McAfee(미국) | 보안 번들 | 소비자 | 5 | 4 | 3 | 영상 96%(벤더 주장), 실제로는 오디오 위주 분석 [McAfee](https://www.mcafee.com/en-us/newsroom/press-releases/2025/mcafees-scam-detector-added-to-core-plans-protecting-people-against-text-email-and-video-scams.html) |
| Norton Genie / Avast | Gen Digital(미국) | 구독 번들 | 소비자 | 5 | 3 | 2 | 영어 YouTube 영상 한정 [Norton](https://support.norton.com/sp/en/us/home/current/solutions/v20250722122612120) |
| YouTube 초상 감지 | Google(미국) | 플랫폼 내장 | 크리에이터 | 5 | 4 | 3 | 진위 판별이 아니라 본인 얼굴 찾기 [Tubefilter](https://www.tubefilter.com/2026/05/18/youtube-generative-ai-deepfake-likeness-detection-rollout/) |
| Gemini SynthID 검증 | Google(미국) | 앱 업로드 | 소비자 | 5 | 4 | 3 | Google 워터마크 영상만 [Android Central](https://www.androidcentral.com/apps-software/ai/gemini-can-now-tell-you-whether-a-video-was-generated-with-google-ai) |
| Zoom·Teams 탐지 | Zoom·MS(미국) | 회의 애드온·연동 | 기업 | 5 | 1 | 2 | 출시 전(2026.12~2027Q1 예상) [Zoom](https://www.zoom.com/en/blog/zoomtopia2026-ai-governance-zoom-workplace/) [BleepingComputer](https://bleepingcomputer.com/news/security/microsoft-teams-to-add-third-party-deepfake-detection-impersonation-protection) |
| 경찰청 SW·국과수 아이기스 | 경찰청·국과수(한국) | 내부 도구 | 수사·선관위 | 4 | 3 | 3 | 누적 1,636건, 국과수 공식 92% [뉴스핌](https://www.newspim.com/news/view/20260813000619) [세계일보](https://www.segye.com/newsView/20260310517457) |
| 딥브레인AI | 딥브레인AI(한국) | SaaS·API | 공공·금융 | 3 | 3 | 3 | 96%는 벤더 의뢰 시험(미확인) [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366) |

국과수 모델 정확도는 요약본끼리 엇갈린다. 영상 요약본은 "단일 92%·앙상블 97%"로, 한국 요약본은 "97%는 기사 제목뿐, 공식 수치는 5종 앙상블 92%"로 적었다. 검증이 더 구체적인 92%를 따른다.

**4개 기준 판정**
- **메이저성: 높음.** 전문 스타트업, 대형 보안사(McAfee·Gen·Bitdefender), 플랫폼(YouTube·Gemini)이 모두 들어와 있고 Gartner가 2026.6 첫 딥페이크 탐지 스타트업 평가를 냈다 [Gartner](https://www.gartner.com/en/documents/8056333). 단 Zoom·Teams 기능은 아직 출시 전이다.
- **완성도·실사용: 중간.** 콜센터·채용·모더레이션 같은 B2B는 실제로 쓰인다. 소비자 독립 도구는 채택이 미미하고, 구글플레이 탐지 앱은 많아야 1만+ 다운로드다 [Google Play](https://play.google.com/store/apps/details?id=com.avk.imagehunter2&hl=en_US). NYT 테스트(12개 서비스)에서 영상이 가장 취약했고 영상을 아예 지원하지 않는 곳도 많았다 [Gigazine](https://gigazine.net/gsc_news/en/20260302-ai-detection-fake).
- **신뢰도: 낮음.** 벤더는 95~99%를 주장한다. 독립 평가에서는 실제 유통 딥페이크 앞에서 오픈소스 탐지기 성능(AUC)이 영상 50% 떨어졌고 상용도 인간 분석가에 못 미쳤다 [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857). 최신 생성기 영상에서 학술 탐지기는 94.3→48.2로 붕괴했다(상용 전체로 일반화는 과장) [DF26](https://arxiv.org/pdf/2609.07369). 선관위도 두 시스템이 모두 딥페이크라고 해야 확정한다 [세계일보](https://www.segye.com/newsView/20260310517457).
- **신규 진입 경쟁력: 범용 낮음, 틈새 중간.** 2026년 투자는 음성·사기·신원 쪽으로 몰렸다 [TechBytes](https://techbytes.app/posts/allure-security-17m-series-b-deepfake-fraud-prevention/). 재학습하면 AUROC 93.1 이상으로 회복된다는 결과가 있어 빠른 데이터 운영이 차별점이 될 수 있다 [DF26](https://arxiv.org/html/2609.07369v1).

**레드오션 판정: 부분적(범용 = 예, 특화 = 아니오)**
- 범용 앱·API는 **예**. 전문 기업, 보안사 번들, RealCheck, 플랫폼 기능이 이미 경쟁하고 인수·통합(Deel–Clarity, KPMG)도 시작됐다 [Calcalist](https://www.calcalistech.com/ctechnews/article/bkeyex0sgl).
- 특화는 **아니오**. 범죄·사고 장면 영상에서 10개 탐지기가 모두 실패했고 [ChatPaper](https://chatpaper.com/chatpaper/paper/357903), 한국어 소비자 도구는 비어 있으며(RealCheck·Norton 영어 전용), 법정 증거 수준은 아직 아무도 못 갖췄다.
- 특허: 영상 탐지 전반을 막는 특허는 없다. 단 얼굴 라이브니스(FaceTec 특허 유지)는 예외라 FTO가 필요하다 [BiometricUpdate](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents).

### 2.3 음성(보이스피싱·딥보이스)

| 제품 | 회사 | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| Pindrop Pulse | Pindrop(미국) | 콜센터 플랫폼·API | 금융·콜센터 | 5 | 4 | 3 | 매출 1억 달러 이상(CEO). 99%는 "이미 아는 엔진" 기준(벤더 주장) [Mergermarket](https://ionanalytics.com/insights/mergermarket/pindrop-could-step-up-acquisitions-in-agentic-security-as-its-deepfake-detection-takes-off-ceo/) [Pindrop](https://www.pindrop.com/article/pindrop-pulse-for-audio-deepfake-detection/) |
| Resemble Detect | Resemble AI(미국) | API | 기업·정부 | 4 | 3 | 3 | Podonos 98.1% 1위(Resemble이 홍보) [Resemble](https://www.resemble.ai/resources/audio-deepfake-detection-benchmark-results-how-8-systems-performed-in-2026) |
| Modulate | Modulate(미국) | 셀프서브 API | 개발자 | 3 | 4 | 2 | 음성 1시간 0.25달러, 2,500만 달러 투자 [TechCrunch](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/) |
| Reality Defender | Reality Defender(미국) | API·무료 티어 | 기업·개발자 | 4 | 3 | 2 | Podonos 71.3%, 오탐 53.7% [SSN](https://www.securitysystemsnews.com/article/reality-defender-launches-public-api-and-free-tier) |
| SynthID Detector | Google(미국) | 무료 웹 | 소비자·언론 | 5 | 3 | 4(자사 한정) | 워터마크 구간 표시, 범용 아님 [Google](https://blog.google/technology/ai/google-synthid-ai-content-detector/) |
| ElevenLabs Audio Detector | ElevenLabs | 무료 웹 | 소비자 | 4 | 2 | 3(자사 한정) | 자사 음성 정밀도 99%·재현율 80%(공식 문서) [ElevenLabs](https://elevenlabs.io/docs/eleven-creative/audio-tools/audio-detector) |
| Hiya·Truecaller | Hiya(미국)·Truecaller(스웨덴) | 통화 앱·확장 | 소비자 | 3 | 2 | 2 | 독립 검증 없음 [Hiya](https://www.hiya.com/press-releases/hiya-acquires-deepfake-voice-detection-leader-loccus-ai) |
| McAfee·Norton | McAfee·Gen(미국) | 보안 번들 | 소비자 | 3 | 2 | 2 | 영어, AI PC·YouTube 한정 [eSecurityPlanet](https://www.esecurityplanet.com/cybersecurity/best-ai-deepfake-detection-tools/) |
| 갤럭시 보이스피싱 알림 | 삼성전자(한국) | OS 기본 기능 | 갤럭시 사용자 | 5 | 5 | 2 | 사용률 약 84%. 합성음 탐지 근거 없음 [바이라인](https://byline.network/2026/04/27-613/) |
| KT 보이스피싱 탐지 | KT(한국) | 통신 서비스·앱 | Android 전체 | 4 | 4 | 3 | 딥보이스 98%(벤더 주장), 3.0은 판단 근거 제공 [디데일리](https://www.ddaily.co.kr/page/view/2025072908585835162) |
| 익시오 안티딥보이스 | LG유플러스(한국) | 온디바이스 | 가입자·국과수 | 4 | 3 | 2 | 98%(벤더 주장), 국과수에 무상 제공 [머니투데이](https://www.mt.co.kr/tech/2025/07/23/2025072315221813011) |
| 에이닷 전화 | SK텔레콤(한국) | 통신사 앱 | 가입자 | 4 | 3 | 2 | 문맥·성문 기반, 합성음 탐지 근거 없음 [바이라인](https://byline.network/2026/04/27-613/) |
| 딥브레인AI·한컴위드 스피키 | 딥브레인AI·한컴위드(한국) | SaaS·화자인증 | 경찰·금융 | 2~3 | 2 | 2 | 성능은 벤더 발표뿐 [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366) [바이라인](https://byline.network/2026/09/11-703/) |

Reality Defender의 KPMG 지분 투자는 음성 요약본이 "미확인"으로 적었지만, KPMG 공식 발표가 있어 확정으로 본다 [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html).

**4개 기준 판정**
- **메이저성: 높음.** 기업 시장은 Pindrop이 선두이고 Zoom·FICO 제휴로 유통을 굳히고 있다 [BiometricUpdate](https://www.biometricupdate.com/202603/zoom-expands-pindrop-deepfake-detection-to-customer-service). 한국은 삼성과 통신3사가 무료 기본 기능으로 제공한다 [바이라인](https://byline.network/2026/02/12-535/).
- **완성도·실사용: 채널을 가진 사업자만 높음.** 삼성 기능은 기본으로 켜져 있다. 단독 소비자 업로드 도구(Hiya, AI or Not)의 사용자 수는 미확인이다. 수요는 크다. 6개국 응답자의 31%가 1년 안에 딥페이크 음성 전화를 받았다(벤더 조사) [Hiya](https://blog.hiya.com/ai-is-making-voice-fraud-worse-both-in-volume-and-in-targeting).
- **신뢰도: 낮음~중간.** 2026년에도 상용 탐지기를 비벤더가 독립 평가한 결과는 찾지 못했다. Podonos 벤치마크(테스트셋 비공개, 1위 벤더가 홍보)에서 상용 71~98%, 오픈소스 48~63%였다 [Podonos](https://www.resemble.ai/resources/audio-deepfake-detection-benchmark-results-how-8-systems-performed-in-2026). 동료심사를 거친 Speech DF Arena는 처음 보는 환경에서 오류율이 높다고 보고했다 [arXiv 2509.02859](https://arxiv.org/pdf/2509.02859). 실제 유통 딥페이크에서 오디오 AUC는 약 48% 떨어진다(독립 평가) [arXiv 2503.02857](https://arxiv.org/abs/2503.02857).
- **신규 진입 경쟁력: 범용 낮음, 니치는 조건부.** Modulate가 1시간 0.07~0.25달러 API를 팔고, Google·Reality Defender는 무료다. 독립 앱은 Google Play 정책 때문에 실시간 통화 접근이 사실상 막혀 있다 [Engadget](https://www.engadget.com/google-is-banning-third-party-call-recording-apps-from-the-play-store-093201443.html). 수사기관용 한국어 감정은 대검(2027년까지 86억 원 R&D)과 국과수가 내재화 중이다 [서울신문](https://m.seoul.co.kr/news/2024/04/01/20240401500181). 비어 있는 것은 민간 분쟁(법무·보험·노동)용 "검증된 감정 리포트" 제품뿐이다 [한경](https://www.hankyung.com/article/2024110369981).

**레드오션 판정: 부분적(대부분 예)**
- 기업 콜센터·소비자 업로드 판별은 **예**. Pindrop·Microsoft·Resemble·Modulate가 경쟁하고 무료 도구가 넘친다. 인수 통합도 시작됐다 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection).
- 한국 실시간 통화 탐지는 **사실상 진입 불가**. 대기업 무료 기능에 OS 정책까지 막고 있다.
- 민간용 한국어 음성 감정 리포트는 **아직 아니지만 좁아지는 중**. 특허는 분야 전체를 막지 않지만 Pindrop(딥페이크 특허 18건 이상 주장)·대검·딥브레인AI 개별 특허는 FTO가 필요하다 [Pindrop](https://pindrop.com/products/liveness-detection).

### 2.4 음악

| 제품 | 회사 | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| Deezer AI 음악 탐지 | Deezer(프랑스) | 내부 태깅·B2B 라이선스·무료 웹 | 스트리밍·권리단체·소비자 | 5 | 4 | 3 | 2026.1 외부 판매(첫 고객 Sacem), 2026.6 무료 도구 [Dataconomy](https://dataconomy.com/2026/01/29/music-streaming-giant-deezer-opens-ai-detection-tool-to-external-platforms/) [Winbuzzer](https://winbuzzer.com/2026/06/12/deezer-opens-free-ai-playlist-scanner-to-rival-services-xcxwbn/) |
| SynthID Detector(Lyria) | Google(미국) | 무료 웹 | 소비자·플랫폼 | 5 | 3 | 4(자사 한정) | Suno 등 비SynthID 곡은 판별 불가 [AI Musicpreneur](https://www.aimusicpreneur.com/ai-tools-news/google-synthid-detector-public-launch-ai-music-october-2026/) |
| Modulate AI 음악 탐지 | Modulate(미국) | API | 개발자·플랫폼 | 3 | 4 | 2 | 음악 1시간 0.07달러 [TechCrunch](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/) |
| IRCAM Amplify AIMD | IRCAM Amplify(프랑스) | B2B API(견적제) | 레이블·유통 | 3 | 2 | 2 | 98.5~99%(벤더 주장), AP 소규모 테스트 81.8~98% [Cyanite](https://cyanite.ai/blog/best-ai-music-detection-tools-2026/) |
| Believe AI Radar | Believe(프랑스) | 유통 내부 도구 | 자사 고객 | 3 | 3 | 2 | 98%(벤더 주장), 2026 현황 미확인 [MBW](https://musicbusinessworldwide.com/believe-has-developed-its-own-ai-made-music-detector-with-98-accuracy-what-might-this-mean-for-the-future) |
| ACRCloud | ACRCloud(해외) | B2B | 국내 권리단체 | 2 | 미확인 | 미확인 | 국내 시연 [위키트리](https://www.wikitree.co.kr/articles/1137778) |
| 국산 제품 | - | - | - | - | - | - | 없음. 음저협이 "한국형 AI 디텍션" 검토 중 [아시아경제](https://view.asiae.co.kr/article/2026083116360854659) |

**4개 기준 판정**
- **메이저성: 높음.** Deezer가 사실상 표준 후보로 외부 판매를 시작했고, Google 워터마크 검증도 생겼다. Spotify는 자체 탐지 대신 자진 신고와 "AI Persona" 라벨로 대응한다 [PPC Land](https://ppc.land/spotify-drops-ai-persona-artists-from-recommendations-in-mid-september/).
- **완성도·실사용: B2B는 높음.** Deezer 일일 업로드의 50% 이상이 AI 곡이고, 85%를 수익화에서 뺐다 [TechCrunch](https://techcrunch.com/2026/07/21/music-streamer-deezer-says-more-than-50-of-daily-uploads-are-ai-generated/). 소비자는 무료 도구가 있다.
- **신뢰도: 중간 이하.** 거의 모두 벤더 주장이다. Deezer 자체 연구도 실험실 99.8%가 피치·템포 변경과 재인코딩에 약하다고 했다 [arXiv 2405.04181](https://arxiv.org/abs/2405.04181), 미확인(사전 지식). "97%가 AI 음악을 구분 못 한다"는 조사는 탐지를 파는 Deezer가 의뢰한 것이다 [Deezer](https://newsroom-deezer.com/2025/11/deezer-ipsos-survey-ai-music/).
- **신규 진입 경쟁력: 낮음.** Deezer 라이선스, Modulate 초저가 API, IRCAM, SynthID와 경쟁해야 한다. 국내 수요(감사원 지적, 저작권료 분쟁)는 있으나 수요자가 해외 솔루션 도입·자체 개발을 서두르고 있다 [주간경향](https://weekly.khan.co.kr/article/202610130600011).

**레드오션 판정: 예(B2B는 사실상 레드오션, 국내는 초기 경쟁)**
- 해외 B2B는 Deezer·Modulate·IRCAM이 가격과 규모를 이미 정했다 [iMusician](https://imusician.pro/en/resources/blog/deezer-demonetizes-85-of-ia-music-commercializes-ia-detection-technology).
- 국내는 국산 제품이 없지만 "빈 시장"이 아니라 "해외 벤더와 경쟁하는 초기 시장"이다. 음저협 AI 곡 등록 기준은 22일 만에 철회돼 수요 주체의 방향도 아직 불확실하다 [아시아경제](https://view.asiae.co.kr/article/2026083116360854659).
- 특허: Deezer 출원 2건은 청구항 미확인이다 [Deezer](https://newsroom-deezer.com/2025/01/deezer-deploys-cutting-edge-ai-detection-tool-for-music-streaming/).

### 2.5 글(텍스트)

| 제품 | 회사 | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| Turnitin AI 탐지·Clarity | Turnitin(미국) | 기관 SaaS·LMS | 대학·학교 | 5 | 5 | 3 | 첫해 2억 건 이상(벤더 데이터). 한국어 미지원 [Wired](https://www.wired.com/story/student-papers-generative-ai-turnitin/) [Turnitin FAQ](https://guides.turnitin.com/hc/en-us/articles/28477544839821-Turnitin-s-AI-writing-detection-capabilities) |
| GPTZero | GPTZero→Superhuman(미국) | 웹·API·확장 | 교사·학생·기관 | 5 | 5 | 4 | 사용자 1,900만+, ARR 3,000만 달러(벤더). 2026.6 인수 발표 [Startup Fortune](https://startupfortune.com/superhuman-bets-on-trust-as-it-buys-ai-detection-startup-gptzero-for-its-19-million-users-and-30m-arr/) |
| Superhuman(구 Grammarly) | Superhuman(미국) | 확장·작성 과정 리포트 | 학생·기업 | 5 | 3 | 2 | GPTZero와 통합 예정 [BetaKit](https://betakit.com/grammarly-rebrands-to-superhuman-as-it-expands-from-catching-typos-to-ai-productivity/) |
| Pangram | Pangram Labs(미국) | 웹·API | 교육·출판 | 3 | 3 | 4 | 독립 평가 3건 최상위 [NBER](https://www.nber.org/system/files/working_papers/w34223/w34223.pdf) |
| OpenAI textGrain | OpenAI(미국) | 생성 시 워터마크 | EU 사용자·연구자 | 5 | 2 | 3 | 2026.10 EU 적용, 검출기는 연구자 한정 [BleepingComputer](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-is-adding-invisible-watermarks-to-chatgpt-and-codex-text-in-the-eu/) |
| Originality.ai | Originality.ai(캐나다) | 웹·API | SEO·출판 | 3 | 3 | 3 | 오탐 3.8%(독립 평가) [Epoch AI](https://epoch.ai/data-insights/ai-detectors-false-negatives) |
| Copyleaks·QuillBot·ZeroGPT 등 | 다수 | 웹·API | 소비자·교육 | 2~4 | 3~4 | 2~3 | 무료 티어 보편. ZeroGPT는 미국 헌법을 AI로 판정 [Ars Technica](https://arstechnica.com/information-technology/2023/07/why-ai-detectors-think-the-us-constitution-was-written-by-ai/) |
| 무하유 GPT킬러 | 무하유(한국) | 웹·기관 플랫폼 | 대학·공공·채용 | 3 | 4 | 2 | 98%(벤더 주장). 대학 유통 장악 [아이티데일리](https://www.itdaily.kr/news/articleView.html?idxno=223370) [지티티코리아](https://www.gttkorea.com/news/articleView.html?idxno=22638) |
| AI킬러 등 소형 탐지기 | 개인·소규모(한국) | 웹 | 학생 | 1 | 1 | 1 | 무료, 자체 주장뿐 [AI킬러](https://aikiller.app/) |
| OpenAI AI Text Classifier | OpenAI(미국) | 웹 | 일반 | 5 | 1 | 1 | 2023.7 종료, 자체 공개 탐지율 26% [OpenAI](https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/) |

**4개 기준 판정**
- **메이저성: 높음.** Turnitin(기관)과 Superhuman+GPTZero(소비자·기관)의 플랫폼 구도가 됐다 [BusinessWire](https://www.businesswire.com/news/home/20260623083788/en/Superhuman-to-Acquire-GPTZero-AI-Authenticity-Platform). 생성사(OpenAI·Google)도 워터마크 검출기를 직접 쥐고 있다.
- **완성도·실사용: 높음.** 다섯 모달리티 중 실사용이 가장 크다. 미국 6~12학년 교사의 68%가 정기적으로 쓴다 [CDT](https://cdt.org/insights/new-research-educators-still-struggling-with-generative-ai-detection-discipline-and-distrust-despite-increased-school-guidance/).
- **신뢰도: 중간, 구조적 한계.** 독립 평가에서 Pangram·GPTZero는 사람 글 오탐이 거의 0이었지만 [NBER](https://www.nber.org/system/files/working_papers/w34223/w34223.pdf), 문체를 흉내 낸 AI 글은 10~29%를 놓쳤다 [Epoch AI](https://epoch.ai/data-insights/ai-detectors-false-negatives). 비원어민 영어 에세이 평균 오탐 61.3%(2023년 도구 기준) [Liang 외](https://arxiv.org/html/2304.02819v3). 탐지 점수 하나로 내린 징계를 법원이 무효화했다(절차 하자 판결) [Plagiarism Today](https://www.plagiarismtoday.com/2026/02/11/adelphi-student-wins-ai-plagiarism-lawsuit/). 대학의 사용 중단도 늘고 있다 [Waterloo](https://uwaterloo.ca/educational-technology-hub/news/discontinuing-use-ai-detection-functionality-turnitin).
- **신규 진입 경쟁력: 낮음.** 유통은 대형사가 묶었고, 정확도 상위는 Pangram·GPTZero가 독식하며, 무료가 기본이다. 한국어는 무하유가 장악했고 Turnitin이 분기마다 언어를 늘리고 있어 공백은 시한부다. 한국어 공개 벤치마크(KatFish)와 코드도 이미 공개돼 "한국어"만으로는 장벽이 안 된다 [ACL Anthology](https://aclanthology.org/2025.acl-long.1030).

**레드오션 판정: 예(영어 범용) / 한국어·수사용 니치는 부분적**
- 주요 제품만 15개가 넘고 대부분 무료 티어가 있다. 2026년 인수로 유통 장벽이 더 높아졌다 [TechCrunch](https://techcrunch.com/2026/06/23/superhuman-acquires-ai-detection-startup-gptzero/).
- 수요 측 역풍: 교육 시장이 "탐지"에서 "작성 과정 증명"으로 옮겨 가고, 학생들은 제출 전 탐지기로 흔적을 지운다(국내 재검사 6.6회→10.7회) [머니투데이](https://www.mt.co.kr/amp/future/2026/05/26/2026052609184984243).
- 막는 것은 특허가 아니라 유통과 신뢰성이다. 구현 방식별 특허는 있어 FTO가 필요하다 [US11853708B1](https://patents.google.com/patent/US11853708B1/en).

### 2.6 통합(멀티모달) 소비자 앱

사용자가 구상하는 "영상·사진·음악·글을 한 곳에 넣으면 판별해 주는 앱"에 가장 가까운 제품들이다.

| 제품 | 회사 | 형태 | 지원 매체 | 메이저성 | 실사용 | 신뢰도 | 비고 |
|---|---|---|---|---|---|---|---|
| Google SynthID Detector | Google(미국) | 무료 웹(영어) | 이미지·영상·오디오(글 제외) | 5 | 4 | 3 | 워터마크 확인만. OpenAI·NVIDIA·Kakao 워터마크도 판독 [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/) |
| Hive AI Detector | Hive(미국) | 크롬 확장·웹 | 이미지·영상·글·오디오 | 4 | 3 | 3 | 사용자 약 5만, 평점 4.6 [Chrome 웹스토어](https://chromewebstore.google.com/detail/hive-ai-detector/cmeikcgfecnhojcbfapbmpbjgllklcbi?hl=fil) |
| Bitdefender RealCheck | Bitdefender(루마니아) | 모바일 앱 | 영상 중심 | 4 | 2 | 2 | 영어 전용, 월 4.99달러 [Gizmodo](https://gizmodo.com/bitdefender-built-an-app-that-analyzes-videos-for-deepfakes-so-you-dont-have-to-guess-2000780027) |
| McAfee·Norton 번들 | McAfee·Gen(미국) | 보안 구독 | 영상 속 음성 위주 | 5 | 3 | 2 | 영어, 특정 기기·YouTube 한정 [SecurityBrief](https://securitybrief.co.uk/story/norton-adds-ai-powered-deepfake-detection-to-genie-assistant) |
| AI or Not | AI or Not(미국) | 웹·앱·API | 이미지·오디오 | 3 | 3 | 2~3 | NPR 음성 테스트에서 약 절반 오판(2024) [NPR](https://www.npr.org/2024/04/05/1241446778/deepfake-audio-detection) |
| Reality Defender 무료 티어 | Reality Defender(미국) | 웹·API | 이미지·오디오(영상 제외) | 4 | 2 | 2~3 | 월 50건 무료 [SSN](https://www.securitysystemsnews.com/article/reality-defender-launches-public-api-and-free-tier) |
| Pangram | Pangram Labs(미국) | 웹·API | 글·이미지(프리뷰) | 3 | 3 | 4(글) | 멀티모달로 확장 중, 구상 앱과 직접 경쟁 [BusinessWire](https://www.businesswire.com/news/home/20260729222515/en/Pangram-Launches-New-Worlds-Best-AI-Detector-Expands-to-Images-Backed-by-$9M-From-Menlo-Ventures) |
| TrueMedia.org | Georgetown(미국) | 웹(클로즈드 베타) | 이미지·오디오 | 2 | 1 | 미확인 | 비영리, 운영비로 2025.1 종료 후 재가동 [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/) |
| FakeCheck 2.0 | 샌즈랩(한국) | 무료 웹 | 얼굴 이미지(영상 가능성) | 2 | 2 | 2 | 99.33%는 미확인 [인공지능신문](https://www.aitimes.kr/news/articleView.html?idxno=34963) |
| 라온 모바일 시큐리티 | 라온시큐어(한국) | 백신 앱 내장 | 얼굴 이미지 | 3 | 2 | 2 | 무료, 성능 미공개 [이투데이](https://www.etoday.co.kr/news/view/2439014) |
| KaiCatch | KAIST 연구팀(한국) | Android 앱 | 이미지 | 2 | 1 | 2 | 2022년 이후 정체 [이데일리](https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=02725686628988568) |

**4개 기준 판정**
- **메이저성: 지배적 단일 브랜드 없음.** 모달리티마다 강자가 나뉘고, 소비자 접점은 빅테크와 보안 번들이 쥐고 있다 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection). 네 매체(영상·사진·음악·글)를 모두 다루는 메이저 소비자 앱은 확인되지 않았다(SynthID Detector는 글 제외, 워터마크 확인만).
- **완성도·실사용: 낮음.** 앱스토어 탐지 앱은 작동하지 않거나 리뷰가 의심스러운 경우가 많다 [Copyleaks](https://copyleaks.com/blog/ai-detector-apps-arent-what-they-claim). 국산 소비자 도구는 얼굴 이미지 중심 무료 부가 기능이고, 해외 앱이 국내 수요를 일부 흡수한다 [jakeinsight](https://jakeinsight.com/ko/tech-economy/2026-09-03-%EB%94%A5%ED%8E%98%EC%9D%B4%ED%81%AC-%ED%83%90%EC%A7%80%EA%B8%B0-%EC%95%B1-%EC%A7%84%EC%A7%9C-%EB%AF%BF%EC%96%B4%EB%8F%84-%EB%90%98%EB%82%98/).
- **신뢰도: 낮음.** 각 모달리티의 한계(2.1~2.5)가 그대로 합쳐진다. 독립 평가에서 실제 유통물 앞에서 오픈소스 탐지기 성능이 영상 50%, 음성 48%, 이미지 45% 떨어졌다 [arXiv 2503.02857](https://arxiv.org/abs/2503.02857).
- **신규 진입 경쟁력: 낮음.** "올인원" 자체는 비어 있는 것처럼 보이지만, 각 칸마다 무료 대체재가 있고 운영비(매 생성기마다 재학습)가 커서 비영리 TrueMedia도 독자 운영을 접었다 [TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia). 차별화 여지는 "워터마크·C2PA·탐지·메타데이터를 한 리포트로 묶는 통합 검증"과 한국어 지원 정도다 [Morgan Lewis](https://www.morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative).

**레드오션 판정: 예(수익 관점)**
- 국산 메이저 통합 앱은 없지만, 무료·번들 대체재(Google, Hive, 보안사, Reality Defender 무료 티어)가 이미 있어 B2C 유료화가 어렵다 [SocialMediaToday](https://www.socialmediatoday.com/news/youtube-expands-likeness-detection-to-all-users-over-18/820440/).
- "범죄까지 잡는 정교한 범용 판별"은 어느 회사도 독립 평가로 입증하지 못한 미해결 기술 문제다. 시장이 비어 있는 이유가 수요 부족이 아니라 기술·비용 한계라는 점에 주의해야 한다.



## 3. 빅테크·출처증명(C2PA, SynthID 등)과 규제

이 절의 요지는 간단하다. **"유명 AI로 만든 콘텐츠인지 확인"하는 기능은 이미 빅테크가 무료로 나눠 주고 있다.** 반면 그 기능이 닿지 않는 영역(워터마크가 없거나 지워진 콘텐츠)은 여전히 비어 있다.

용어부터 정리한다.
- **워터마크(SynthID 등):** AI가 콘텐츠를 만들 때 눈에 안 보이는 표식을 심어 두는 방식이다. 표식을 심은 회사(또는 협조한 회사)의 콘텐츠만 확인할 수 있다.
- **출처증명(C2PA, Content Credentials):** 파일에 "누가, 어떤 기기·프로그램으로 만들었고 어떻게 편집했는지"를 전자서명으로 붙이는 국제 표준이다. 로열티 프리다 [C2PA FAQ](https://www.c2pa.org/faq).
- 두 방식 모두 **사후 탐지(콘텐츠 자체를 분석해 AI 흔적을 찾는 것)가 아니다.** 표식이 없으면 아무 말도 못 한다.

### 3.1 빅테크의 무료 확인 기능

| 기능 | 회사 | 형태·대상 | 현재 상태 | 한계 |
|---|---|---|---|---|
| SynthID Detector 포털 | Google | 무료 웹, 소비자·언론 | 2026-10-07 전 세계 공개(영어) [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/) | 협조사 워터마크만 판정, 오류율 비공개 |
| Search·Chrome·Circle to Search 확인 | Google | 검색·브라우저 기본 기능 | SynthID 2026-05부터 배포 [Google I/O](https://blog.google/innovation-and-ai/technology/ai/io-2026-keynote-moment-videos/) | C2PA 지원은 예정 |
| Gemini 앱 확인 | Google | 앱 기능 | 이미지·영상 지원 | 한 대화 안에서 판정이 엇갈린 사례(팩트체크 미확인) [Lead Stories](https://leadstories.com/analysis/2026/07/google-gemini-synthid-detector-confuses-results-within-same-chat.html) |
| AI Content Detection API | Google | 기업용 API | 2026-05 제한 프리뷰 [InfoQ](https://infoq.com/news/2026/05/google-synthid-content-detection) | 신뢰도 미확인 |
| YouTube 자동 AI 라벨·초상 탐지 | Google | 플랫폼 내장 | 2026-05 자동 라벨 [MBW](https://www.musicbusinessworldwide.com/youtube-will-now-automatically-detect-and-label-ai-videos-even-when-creators-dont-disclose-it/) | 정확도 비공개 |
| OpenAI Verify | OpenAI | 웹 도구 | Research preview(이미지 2026-05-19~) [OpenAI 도움말](https://help.openai.com/en/articles/8912793-c2pa-in-chatgpt-images) | 자사 산출물 전용 |
| Meta AI info 라벨·Content Seal | Meta | 플랫폼 라벨·탐지 프리뷰 | 2026-07 프리뷰 | 자르기만 해도 55% 놓침(독립 평가) [The Star](https://www.thestar.com.my/tech/tech-news/2026/07/10/meta-ai-image-detector-fails-to-identify-some-of-its-own-cropped-ai-images-reuters-analysis-finds) |
| TikTok AIGC 라벨·워터마크 | ByteDance | 플랫폼 내장 | 2025-11 테스트 | TikTok 안에서만 읽힘 [TechCrunch](https://techcrunch.com/2025/11/18/tiktok-now-lets-you-choose-how-much-ai-generated-content-you-want-to-see/) |
| ElevenLabs Audio Detector | ElevenLabs | 무료 웹 | 2026-07 SynthID 적용 [ElevenLabs](https://elevenlabs.io/blog/synthid) | 자사 음성만 판정 |
| Adobe Content Authenticity | Adobe | 웹 앱·Chrome 확장 | 퍼블릭 베타 [Adobe](https://helpx.adobe.com/ae_en/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html) | 자격증명 붙은 콘텐츠만 의미 |
| Pixel 10 / Galaxy / Apple 카메라 서명 | Google·Samsung·Apple | 촬영 기기 서명 | Pixel 10 전 JPEG 서명, Apple Reference Image는 2026-09 iPhone 18 Pro [Nieman Lab](https://www.niemanlab.org/2026/09/apple-launches-a-new-way-to-prove-a-photo-was-shot-with-an-iphone-not-generated-by-ai/) | "진짜 증명"용, 탐지기 아님. Apple은 C2PA 아님 |

SynthID 연합에는 OpenAI, NVIDIA, Kakao, ElevenLabs가 참여했고 Apple은 "곧" 참여한다(날짜 미공개) [Mixed](https://mixed-news.com/en/google-synthid-detector-worldwide-apple-ai-content-comes-soon/). Google은 이미지·영상 1천억 건 이상에 SynthID를 넣었다고 밝혔다(벤더 주장) [InfoQ](https://infoq.com/news/2026/10/synthid-watermarking-detector). 다만 **어느 회사도 확인 도구 이용자 수를 공개하지 않는다.** 생태계는 쪼개져 있다. Meta, Microsoft, TikTok은 각자 워터마크를 쓰고, Microsoft 워터마크는 SynthID와 호환되지 않는다 [arXiv 2602.18681](https://arxiv.org/abs/2602.18681).

### 3.2 워터마크·출처증명의 한계

| 한계 | 내용 | 근거 |
|---|---|---|
| 업로드하면 사라짐 | WaPo가 C2PA가 든 영상을 8개 플랫폼에 올렸더니 모두 자격증명을 보존·표시하지 않음(2025-10 테스트, 독립 평가) | [AIID](https://incidentdatabase.ai/reports/6301) |
| 쉽게 제거 | Galaxy의 C2PA 라벨은 exiftool 같은 도구로 쉽게 지워짐 | [PetaPixel](https://petapixel.com/2025/02/13/samsungs-image-authenticity-approach-is-backward-and-its-ais-fault) |
| 재생성 공격 | 이미지를 AI로 한 번 더 다시 그리면 SynthID가 무력해짐(독립 평가) | [AI Weekly](https://aiweekly.co/alerts/google-synthid-watermarks-hold-up-in-tests-labeling-still-slips) |
| 단순 편집에도 실패 | Meta 탐지기: 원본 40장은 다 잡았지만 잘린 이미지는 55% 놓침(Reuters, 표본 40장) | [Gizmodo](https://gizmodo.com/metas-ai-detector-cant-detect-images-it-generated-itself-report-finds-2000784335) |
| 글은 더 약함 | 텍스트 워터마크는 문장만 바꿔 써도 98.3% 제거, 사람 글 오탐 5.4%(재현 안 된 프리프린트) | [arXiv 2607.16010](https://arxiv.org/abs/2607.16010) |
| 기기 구현 결함 | Nikon Z6III는 위조 서명 취약점으로 인증서 전량 폐기(팩트체크 미확인) | [DCW](https://www.digitalcameraworld.com/photography/photojournalism/nikon-revokes-all-c2pa-image-authenticity-certificates-after-major-vulnerability-exposed) |
| 오픈소스 모델은 처음부터 밖 | Wan 2.x 같은 오픈웨이트 모델 산출물에는 워터마크가 아예 없음 | [arXiv 2512.11815](https://arxiv.org/abs/2512.11815v2) |
| "미검출 ≠ 사람이 만듦" | 각 회사가 스스로 이렇게 밝힘. 한국 정부도 개인이 워터마크를 지워도 위반이 아니라고 해석 | [다음](https://v.daum.net/v/20260121120209717) |

Microsoft의 자체 보고서(2026-02)도 **"단일 기술로는 믿을 만하게 구별할 수 없다"**고 결론 내렸다 [The Decoder](https://the-decoder.com/microsofts-research-argues-ai-media-authentication-doesnt-work-reliably-yet-new-laws-assume-it-does/).

정리하면 워터마크는 "협조하는 회사가, 원본 그대로 유통된 콘텐츠"에만 통한다. **범죄자는 바로 이 조건을 피해 간다.** 오픈소스 모델을 쓰거나, 캡처·재압축·재생성으로 표식을 지운다. 사용자가 노리는 "범죄 수준" 판별은 워터마크로는 해결되지 않는다.

### 3.3 주요 규제

| 국가·법 | 핵심 내용 | 시행일 | 앱 개발자에게 주는 의미 |
|---|---|---|---|
| 한국 AI 기본법 | AI 생성물 표시 의무(사업자만). 딥페이크가 아니면 비가시 워터마크도 허용 [뉴시스](https://www.newsis.com/view/NISX20260121_0003485509) | 2026-01-22 | 과태료 최대 3천만 원·계도기간 1년(이상) [ZDNet](https://zdnet.co.kr/view?no=20261020095628). 단, 한국 요약본은 이 수치를 미확인으로 봄. 실제 과태료는 2027년 이후 |
| 한국 성폭력처벌법(딥페이크) | 허위영상물 소지·시청까지 처벌(최고 3년) [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877) | 2024-10 개정 | 수사 수요는 크지만, 실제 성범죄 딥페이크를 학습데이터로 모으기 어려움 |
| 한국 공직선거법 | 선거운동에 딥페이크 전면 금지 [트위그](https://www.twig24.com/news/2026/02/11/20260211500394) | 2026-03-05 | 선관위 수요. 단 정부 모델을 무상으로 받아 씀 |
| EU AI Act 50조 | AI 생성물 표시·기계판독 표식 의무 [William Fry](https://www.williamfry.com/knowledge/eu-ai-act-omnibus-deal-reached-postponed-deadlines-watermarking-compromise-and-the-nudificiation-prohibition/) | 2026-08-02(기존 시스템의 2항만 2026-12-02까지 유예, 옴니버스 관보 게재 미확인) | 실천강령 서명사(약 190곳)는 2027-02-02까지 워터마크 탐지 상호운용성 구현 [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/technology-quotient/eu-ai-act-unpacked-33-the-final-code-of-practice-on-transparency-of-ai-generate-102n4yx) |
| EU 누디파이 금지 | 누드 합성·CSAM 생성 AI 금지 [Simmons](https://www.simmons-simmons.com/en/publications/cmoveo6ke00icuxskpgueb0od/ai-omnibus-update) | 2026-12-02 | 플랫폼 탐지 수요 |
| 미국 TAKE IT DOWN Act | 비동의 성적 이미지 신고 시 48시간 내 삭제, 위반 건당 최대 53,088달러 [FTC](https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-sends-warning-letters-companies-about-compliance-take-it-down-act) | 2026-05-19 FTC 집행 | 플랫폼용 탐지·중복 제거 수요 |
| 캘리포니아 SB 942 / AB 853 | 생성 AI 제공자에게 표시·무료 검증도구 의무, 위반 건당·일당 5,000달러 [MoFo](https://www.mofo.com/resources/insights/261001-california-revamps-ai-transparency-requirements) | 2026-08-02 | "생성기별 확인"은 법으로 무료화됨 |
| 캘리포니아 SB 1000 | 100만 명 기준 삭제(모든 생성 AI 제공자 대상). "자격 있는 제3자 검증도구"로도 의무 이행 가능 [Latham](https://www.lw.com/en/insights/newest-slate-of-ai-laws-keeps-california-at-the-forefront-of-us-regulation) | 2026-09-30 서명·즉시 시행(공식 기록 미확인) | 소규모 생성 AI 업체용 화이트라벨 검증도구 B2B 기회 |
| 중국 AI 생성물 표시 규정 | 명시·잠재 표시 의무. 2026-02 13,421개 계정 처벌(팩트체크 미확인) [TechNode](https://technode.com/2026/02/13/china-cyberspace-regulators-crack-down-on-unlabeled-ai-generated-content-penalize-over-13000-accounts/) | 2025-09-01 | 중국 시장은 자국 기업 중심 |
| 덴마크 법안 L 49 | 얼굴·목소리 보호, 게시자에게 입증 책임 [Euronews](https://www.euronews.com/2026/10/08/denmark-introduces-a-bill-protecting-peoples-faces-and-voices-from-deepfakes) | 미통과 | 통과 시 출처 증명 수요 |

주의할 점이 있다. 미국은 연방 행정명령이 주법을 견제하고 있어 주 규제의 앞날이 불확실하다 [Ropes & Gray](https://www.ropesgray.com/en/insights/alerts/2025/12/trump-attempts-to-preempt-state-ai-regulation-through-executive-order). 규제의 대부분은 **생성하는 쪽(AI 제공자·플랫폼)에 표시 의무**를 지운다. 일반인이 "이게 AI인지" 확인할 수 있게 하는 도구는 그 의무의 일부로 빅테크가 직접 무료 제공하게 된다.

### 3.4 결론: 위협인가 기회인가

**소비자 앱으로는 위협, 틈새 B2B로는 조건부 기회다.**

| 구분 | 판정 | 이유 |
|---|---|---|
| "유명 AI로 만들었는지" 확인하는 소비자 앱 | **위협(사실상 끝남)** | Google·OpenAI·ElevenLabs가 무료 제공, Search·Chrome·Gemini·YouTube에 기본 탑재, 캘리포니아 법이 생성사에 무료 검증도구를 의무화 [Morgan Lewis](https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative) |
| 워터마크·C2PA를 직접 만드는 것 | **무의미** | 표준과 연합이 이미 있음. 소규모 팀이 끼어들 자리가 없음 |
| 워터마크 없는/지워진 콘텐츠의 사후 탐지 | **빈 영역이지만 블루오션 아님** | 실전 성능이 크게 떨어지고(4절), 경찰청 자체 도구와 Google 기업용 API가 경쟁자 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364) |
| 여러 표식을 한 번에 확인 + 사후 탐지 결합 | **조건부 기회** | SynthID·Meta·Microsoft·C2PA·Apple이 쪼개져 있음. 다만 EU 상호운용성 기한(2027-02-02) 이후 대형사가 직접 구현하면 흡수될 수 있음 |
| SB 1000 제3자 검증도구(화이트라벨) | **조건부 기회** | 소규모 생성 AI 업체가 고객. 검증도구는 개인정보를 동의 없이 내보내면 안 됨 [Sheppard](https://www.sheppard.com/insights/blogs/california-enacts-ai-spokespeople-chatbots-and-content-disclosures-laws) |
| "원래 없음"과 "지워짐"을 구분하는 제거 흔적 탐지 | **연구 단계 기회** | 오탐률 1%에서 98% 넘게 탐지했다는 프리프린트가 있으나 동료 심사 전, 처음 보는 제거 도구에는 미검증 [arXiv 2605.09203](https://arxiv.org/pdf/2605.09203) |

추가 제약도 있다. OpenAI 약관은 워터마크를 역공학하려는 반복 질의를 금지한다 [OpenAI](https://openai.com/index/advancing-content-provenance). 출처증명 영역에는 특허 분쟁(KeeeX v. C2PA)도 걸려 있다(6절).

한 줄 요약: **빅테크는 "착한 사용자가 만든 표시된 콘텐츠"를 무료로 확인해 준다. 남는 시장은 "나쁜 사용자가 표시를 지운 콘텐츠"인데, 이것이 기술적으로 가장 어렵다.**


## 4. 신뢰도의 현실과 '범죄 수사 수준'의 의미

요지: **실제 환경에서 혼자서 감정 근거가 될 만큼 정확한 AI 판별기는 아직 세계 어디에도 없다(독립 평가).** 수사 현장에서는 AI 판별기를 "1차 선별(스크리닝)" 용도로만 쓰고, 최종 판단은 여러 기법과 사람 전문가가 내린다.

### 4.1 독립 벤치마크 결과

**실제 유통 딥페이크로 시험하면 성능이 반토막 난다.** Deepfake-Eval-2024는 88개 사이트, 52개 언어에서 실제로 퍼진 딥페이크(영상 45시간, 음성 56.5시간, 이미지 1,975장)로 탐지기를 시험했다 [arXiv](https://arxiv.org/abs/2503.02857).

| 평가 | 결과 | 구분 |
|---|---|---|
| Deepfake-Eval-2024 | 오픈소스 최신 탐지기 AUC가 학술 벤치마크 대비 영상 50%, 음성 48%, 이미지 45% 하락. 상용 모델은 오픈소스보다 낫지만 사람 포렌식 분석가에 못 미침 [HF Papers](https://huggingface.co/papers/2503.02857) | 독립 평가 |
| 같은 벤치마크 2차 집계 | 최고 상용 영상 탐지기 정확도 약 78% [EmergentMind](https://www.emergentmind.com/topics/deepfake-eval-2024) | 독립 평가(원문 대조 미확인) |
| DailyBench | 기존 세트(GenImage)에서 90% 넘던 탐지기가 최신 이미지에선 약 57% [DailyBench](https://arxiv.org/pdf/2607.24016) | 독립 평가 |
| 음성 일반화 | 실험실 데이터(ASVspoof 2019)로 학습한 모델의 오류율(EER)이 실제 녹음에서 200~1000% 악화 [Müller 2022](https://arxiv.org/pdf/2203.16263) | 독립 평가 |
| NIST 정부 벤치마크 | 이미지 판별 파일럿 진행, 2026-11 현재 공개 수치 없음 [NIST](https://ai-challenges.nist.gov/t2i) | 독립 평가(결과 비공개) |

AUC는 "진짜와 가짜를 얼마나 잘 가르는지"를 나타내는 점수다. 0.5면 동전 던지기와 같다.

**언론 감사: 오탐을 줄이면 미탐이 늘고, 그 반대도 마찬가지다.** NewsGuard는 진짜 사진 15장과 조작 사진 15장으로 시험했다(2026-05, 표본이 작음) [NewsGuard](https://www.newsguardtech.com/?p=33448).

| 도구 | 진짜 사진을 가짜로 오판(오탐) | 조작 사진 탐지율 |
|---|---|---|
| ScamAI | 40% | 80% |
| ZeroGPT | 20% | 93.3% |
| AI or Not | 6.7% (리터치 사진도 87%를 AI로 판정) | 100% |
| Hive | 0% | 73% (가벼운 리터치는 27%) |
| Sightengine | 0% | 33% |

NYT(2026-02)가 12개 서비스를 비교했을 때, 복잡한 AI 이미지를 맞힌 곳은 AI or Not, Gemini Pro, Hive, Resemble.ai 4곳뿐이었다. 음성은 Sensity와 Resemble.ai가 최상위였다 [The Star(NYT)](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work). 범용 AI 챗봇 7종은 보도사진 10장의 출처 검증에 모두 실패했다 [CJR](https://www.cjr.org/tow_center/why-ai-models-are-bad-at-verifying-photos.php).

**벤더 주장과 독립 평가의 차이.**

| 대상 | 벤더(자체) 주장 | 독립 평가 |
|---|---|---|
| Intel FakeCatcher | 정확도 96% | BBC 테스트에서 진짜 영상을 여러 번 오탐 [PetaPixel](https://petapixel.com/2023/08/02/deepfake-detection-software-analyzes-a-persons-blood-flow) |
| 국과수·행안부 모델 | 76%→92%(정부 발표, 한 매체는 97%로 보도) [세계일보](https://www.segye.com/newsView/20260310517457) | 없음 |
| 경찰청 탐지 SW | 탐지율 약 80%, 수사 참고용 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364) | 없음 |
| Resemble·Modulate | 98%, 98.9% 등. 둘 다 "리더보드 1위" 주장 [SiliconANGLE](https://siliconangle.com/2025/12/08/resemble-ai-hauls-13m-different-approach-deepfake-detection/) | 없음(주장끼리 충돌) |

### 4.2 근본 한계 네 가지

| 한계 | 쉽게 말하면 | 근거 |
|---|---|---|
| 일반화 실패 | 학습 때 본 생성기는 잘 잡지만, 새 생성기가 나오면 성능이 뚝 떨어진다. 계속 다시 학습해야 하고 그 비용이 구조적으로 든다 | [DailyBench](https://arxiv.org/pdf/2607.24016) |
| 압축·변형 | 메신저 전송, 캡처, 해상도 축소만으로도 흔적이 지워진다. 해상도를 낮추고 끝을 자르자 판정이 뒤집힌 사례가 있다 | [Reuters Institute](https://reutersinstitute.politics.ox.ac.uk/news/spotting-deepfakes-year-elections-how-ai-detection-tools-work-and-where-they-fail) |
| 의도적 우회 | 탐지기를 속이도록 설계한 공격(TIGA)은 0.25배로 줄여도 우회율 78%를 유지했다. 상용 Hive도 이미지 조작으로 우회된다는 연구가 보도됐다 | [TIGA](https://arxiv.org/pdf/2604.09706v1), [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive) |
| 오탐 | 진짜 참상 사진이 조작으로 판정된 사례가 있다. 오탐은 명예훼손이나 부당 수사로 이어질 수 있다 | [PhotoWorkout](https://www.photoworkout.com/?p=222434) |

여기에 **"거짓말쟁이의 배당"** 문제가 겹친다. 탐지기가 있으면 진짜 증거도 "AI로 만든 것"이라고 우길 수 있다. 김수현 녹취 사건에서 국과수가 "판정 불가"를 회신하자 한쪽이 이를 "완승"으로 선전했다 [한국경제](https://www.hankyung.com/article/2025121553117). 판정 불가의 사유는 탐지 기술이 아니라 **원본이 아니고 잡음이 많다는 것**이었다 [뉴데일리](https://www.newdaily.co.kr/site/data/html/2025/12/15/2025121500350.html). 수사에서는 판별 정확도만큼 원본 확보와 출처 관리가 중요하다는 뜻이다.

### 4.3 법정 증거로 쓰이려면 무엇이 필요한가

| 요건 | 의미 | 현재 상황 |
|---|---|---|
| 오류율 공개 | 얼마나 자주 틀리는지 숫자로 밝혀야 한다(미국 Daubert/Rule 702 기준) | 빅테크도 오류율을 공개하지 않음 [arXiv 2602.18681](https://arxiv.org/abs/2602.18681) |
| 재현성 | 같은 파일을 넣으면 언제나 같은 결과가 나와야 한다. 모델 버전도 기록해야 한다 | Amped가 결과에 모델 버전 컬럼을 추가 [Amped 40165](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165). Gemini는 한 대화 안에서도 판정이 엇갈린 사례(미확인) |
| 설명가능성 | "AI 확률 87%"가 아니라 근거(주파수, 센서 노이즈, 메타데이터, 조명·기하, 립싱크 등)를 보여 줘야 한다 | 소비자 도구는 대부분 점수만 제공 |
| 증거 보관 연속성 | 파일 해시, 처리 이력(chain of custody)을 남겨 중간에 바뀌지 않았음을 입증 | 김수현 사건처럼 원본이 없으면 판정 자체가 불가 |
| 기관 인정 | ISO/IEC 17025 인정, SWGDE·ENFSI 가이드라인 준수 | 미확인(사전 지식) |
| AI 증거 전용 규칙 | 미국 연방증거규칙 Rule 707 신설 추진 | 2026년 두 차례 보류. 시행은 빨라야 2029-12-01 [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence), [uscourts.gov](https://www.uscourts.gov/sites/default/files/document/advisory_committee_on_evidence_rules_may_2026.pdf) |

실제 판례도 이를 보여 준다. 캘리포니아 Mendones v. Cushman & Wakefield(2025-09)에서 법원은 원고가 낸 영상을 딥페이크로 판단해 소송을 기각했다. 근거는 **AI 탐지 점수가 아니라, 같은 인물이 나온 진짜 증거와의 비교**였다(1심이라 구속력 있는 선례는 아님) [Volokh](https://reason.com/volokh/2025/09/25/court-throws-out-case-after-finding-plaintiffs-submitted-deepfake-videos-and-altered-images/).

### 4.4 포렌식 업계 도구 현황

수사기관이 실제로 쓰는 도구들도 AI 판별을 "보조"로만 다룬다.

| 도구 | 회사(국가) | 대상 | AI 판별의 위치 | 근거 |
|---|---|---|---|---|
| Amped Authenticate | Amped(이탈리아) | 수사기관·감정인 | "스크리닝용"이라고 명시, 결과에 모델 버전 기록. 2026-06 영상 확산모델 탐지 추가 | [Amped 40960](https://blog.ampedsoftware.com/2026/06/25/authenticate-update-40960) |
| Magnet Verify + Axiom Copilot | Magnet Forensics(캐나다/미국) | 수사기관 | "탐지보다 인증(파일 구조 분석)". "100% 신뢰할 딥페이크 탐지는 없다"고 밝힘 | [Magnet](https://www.magnetforensics.com/blog/the-deepfake-detector-paradigm-shift-the-case-for-media-authentication-in-court/) |
| Cellebrite | Cellebrite(이스라엘) | 수사기관 | 전용 딥페이크 탐지 기능은 검색에서 확인 안 됨(확정 아님) | [Forensic Focus](https://www.forensicfocus.com/?p=507588) |
| Hive | Hive(미국) | 플랫폼·국방 | 미 국방부 DIU 2년 240만 달러 프로토타입 계약(성능 검증 아님) | [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive) |
| GetReal Security | GetReal(미국, Hany Farid) | 기업 보안·정부 | 포렌식 SaaS. 공개 성능 데이터 없음 | [GetReal](https://www.getrealsecurity.com/resources/getreal-security-raises-17-5m-series-a-led-by-forgepoint-capital-to-address-rapidly-growing-threats-associated-with-generative-ai-and-malicious-digital-media) |
| 국과수·행안부 모델(아이기스 등) | 정부(한국) | 경찰·선관위 | 5종 앙상블. 선관위는 기존 프로그램과 국과수 모델이 **둘 다** 딥페이크라 할 때만 확정(AND 규칙) | [뉴스1](https://www.news1.kr/amp/local/moi/6096576) |
| 경찰청 판별 시스템 | 숭실대 컨소시엄·한컴위드 등(한국) | 전 수사기관 | 3년 91억 원 국책과제(2025-04~2027-12). 완료 후 수사기관 공동 시스템 계획 | [디지털데일리](https://www.ddaily.co.kr/page/view/2025020211334778803), [바이라인네트워크](https://byline.network/2025/06/5-299/) |

경찰청은 2024년 자체 탐지 SW를 만들어 쓰고 있다. 활용 건수는 요약본끼리 엇갈린다. 한쪽은 "수사 1,636건 활용"으로 적었고 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364), 시장 요약본은 이를 확인하지 못해 빼고 "집중단속 기간 범죄 1,553건 집계, 2026년 1~7월 419명 검거"만 확인된 수치로 남겼다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=134010).

### 4.5 "범죄까지 알아보는 정교한 모델"에 대한 현실 진단

**가능한 것**
- 특정 조건에서의 높은 정확도: 정해진 생성기, 정해진 도메인(예: 한국어 보이스피싱 음성, 보험 청구 사진), 원본에 가까운 파일이라면 높은 성능을 낼 수 있다.
- 1차 선별(트리아지): 수많은 파일 중 사람이 먼저 봐야 할 것을 골라 주는 역할. 수사기관·언론이 실제로 원하는 용도다 [Amped 40165](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165).
- 근거를 보여 주는 리포트: 메타데이터, 편집 흔적, 원본 여부, 출처 표식(C2PA·SynthID) 확인을 한 장에 묶는 것.
- "진짜 / 가짜 / 판정 불가" 3단 출력과 공개 오류율: 오탐을 줄이고 신뢰를 얻는 정직한 방식이다. 선관위 AND 규칙처럼 교차검증용 보조 모델로 들어갈 여지도 있다 [뉴스1](https://www.news1.kr/amp/local/moi/6096576).

**불가능한 것(현재 기술로)**
- 모든 생성기·모든 변형에 대해 "이건 AI다/아니다"를 확정하는 것. 독립 평가에서 어떤 상용 도구도 실전에서 사람 분석가를 넘지 못했다 [arXiv](https://arxiv.org/abs/2503.02857).
- 탐지 점수 하나로 법정 증거를 만드는 것. 판례도 탐지 점수가 아니라 비교 증거로 판단했다 [Volokh](https://reason.com/volokh/2025/09/25/court-throws-out-case-after-finding-plaintiffs-submitted-deepfake-videos-and-altered-images/).
- 새 생성기가 나와도 성능이 유지되는 것. 재학습이 끝없이 필요하다 [DailyBench](https://arxiv.org/pdf/2607.24016).

**소규모 팀이 도달 가능한 수준**

| 목표 | 도달 가능성 | 이유 |
|---|---|---|
| 범용 "AI 확률" 앱 | 가능하지만 의미 없음 | 레드오션. 무료 대체재와 통합 단계 시장 |
| 국과수·경찰 수준의 감정 시스템 | 매우 어려움 | 정부가 91억 원 과제로 자체 개발 중. 실전 범죄 데이터는 법적으로 모으기 어려움 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877) |
| 도메인 특화 + 설명형 리포트 + 공개 오류율 | **현실적 목표** | 보험·법무·언론·학교 1차 선별처럼 좁은 영역. 오픈소스(TrueMedia, MIT)와 상용 API를 묶는 앙상블도 가능 [TrueMedia 오픈소스](https://www.truemedia.org/post/open-source-release) |

결론: **"범죄까지 알아보는 정교한 모델"은 세계 최고 기업과 정부도 아직 도달하지 못한 목표다.** 소규모 팀이 이를 약속하면 오탐·미탐 책임 위험만 커진다. 정직한 목표는 "수사관·감정인이 더 빨리, 근거를 갖고 판단하도록 돕는 도구"다.


## 5. 한국 시장

### 5.1 피해 규모(통계)

| 지표 | 수치 | 출처 |
|---|---|---|
| 딥페이크 성범죄(2024.11~2025.10) | 발생 1,827건, 검거 1,438명(구속 72명), 피의자 중 10대 61.8% | [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877) |
| 딥페이크 피의자 검거(2026.1~7) | 419명(구속 17명) | [뉴데일리](https://www.newdaily.co.kr/site/data/html/2026/08/13/2026081300088.html) |
| 디지털성범죄피해자지원센터 합성·편집 피해 | 2023년 423건 → 2024년 1,384건 | [경향](https://www.khan.co.kr/article/202504111006011) |
| 서울시 디지털성범죄 삭제지원 | 2022년 2,509건 → 2025년 15,777건(단일 출처) | [한국경제](https://www.hankyung.com/article/202603023306i) |
| 방심위 딥페이크 시정요구 | 월평균 1,519건 → 3,789건(2024.8 대책 이후) | [세계일보](https://www.segye.com/newsView/20250107509236) |
| 학교 딥페이크(2024.1~9) | 신고 504건, 피해자 833명, 수사의뢰 417건 | [세계일보](https://www.segye.com/newsView/20240930510518) |
| 선관위 딥페이크 삭제요청 | 2024 총선 388건 → 2025 대선 10,510건 → 2026 지선 10,319건(5.27까지, 최종 미확인) | [경향](https://www.khan.co.kr/article/202605281700001/) [파이낸셜뉴스](https://www.fnnews.com/news/202605281717397963) |
| 보이스피싱 피해액 | 2024년 8,545억 원 → 2025년 1조 2,578억 원(+47.2%), 기관사칭형 78.6% | [아이뉴스24](https://www.inews24.com/view/2008688) |

읽을 때 주의할 점:
- 딥페이크 성범죄 건수는 기관마다 집계가 다르다. 파이낸셜뉴스는 같은 시기를 1,553건으로 집계했다 [파이낸셜뉴스](https://www.fnnews.com/news/202512101835084302).
- **딥보이스(AI 합성 음성)를 쓴 보이스피싱만 따로 센 공식 통계는 없다.** 피해액 1조 원은 보이스피싱 전체 수치다.
- 수요 둔화 신호도 있다. 2026년 집중단속 중간발표에서 허위영상물 범죄가 줄었다 [한국경제](https://www.hankyung.com/article/2026061601621). 보이스피싱 피해액이 2025.10~2026.7에 약 43% 줄었다는 수치는 음성 요약본이 [뉴시스](https://mobile.newsis.com/view/NISX20260604_0003655990)를 근거로 적었지만, 한국 요약본 검증에서는 재확인되지 않았다(미확인).
- 피해는 크고 빠르게 늘었지만, 이것이 곧 "판별 앱 시장"을 뜻하지는 않는다. 아래에서 보듯 탐지 수요의 상당 부분을 정부와 대기업이 무료로 흡수하고 있다.

### 5.2 정부·공공이 직접 보유한 탐지 역량과 예산

| 기관·시스템 | 내용 | 규모·성능 | 출처 |
|---|---|---|---|
| 경찰청 딥페이크 탐지 SW | 2024.3 도입(1차 딥브레인AI 협력, 고도화는 대학·한컴위드). 탐지 SW·AI 전문분석관·범행도구 분석의 "3중 대응" | 누적 1,636건 활용(2026.8, 시장 요약본은 미확인 처리, 4.4 참고), 도입 당시 탐지율 약 80%(2024 정부 발표, 재확인 안 됨) | [뉴데일리](https://www.newdaily.co.kr/site/data/html/2026/08/13/2026081300088.html) [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364) |
| 경찰 R&D | 허위조작 콘텐츠 복합 탐지기술(2025~2027). 끝나면 전 수사기관 공동 시스템 계획 | 91억 원 | [데일리안](https://www.dailian.co.kr/news/view/1408429/) [korea.kr](https://www.korea.kr/news/policyNewsView.do?newsId=148973649) |
| 국과수·KETI 아이기스 | 선거·감정용 정부 모델, 선관위에 무상 지원 | 공식 정확도 92%(5종 앙상블), 2025 대선 감정 15건 | [세계일보](https://www.segye.com/newsView/20260310517457) [세계일보](https://www.segye.com/newsView/20250730515766) |
| 선관위 3단계 감별 | 시청각 탐지 → 아이기스 등 교차검증 → 전문가 감별 | 딥페이크 전용 예산 "전무" | [트위그](https://www.twig24.com/news/2026/02/11/20260211500394) [다음](https://v.daum.net/v/6VGDUSx2ab) |
| 대검찰청 | 합성음성 탐지 자체 개발·특허 출원, 2026.5 AI 위조 탐지 시스템 착수 | 2027년까지 86억 원 R&D | [서울신문](https://m.seoul.co.kr/news/2024/04/01/20240401500181) [한경](https://www.hankyung.com/article/2026050722651) |
| 국과수 음성 | LG유플러스 딥보이스 탐지 시스템을 무상으로 받아 사용 | 보이스피싱 분석 효율 16배(기관 발표) | [머니투데이](https://www.mt.co.kr/tech/2025/07/23/2025072315221813011) |
| IITP 딥페이크 범죄대응 R&D | 2026 ETRI(변환억제)·KETI(정밀탐지) 주관, 유통차단·데이터검증 과제는 2027년 시작 | 2030년까지 300억 원 | [디데일리](https://www.ddaily.co.kr/page/view/2026051314145159743) |
| 서울시 AI 삭제지원 | 성착취물 탐지에서 삭제신고까지 자동화 | 6분 | [서울시](https://mediahub.seoul.go.kr/archives/2014517) |
| 정부 범죄 음성 데이터 | 과기정통부·국과수 등이 실제 범죄 음성을 통신사 학습용으로 지원 | 통신사 탐지 정확도 90.3%→97.2%(2025, 정부 발표) | [바이라인](https://byline.network/2026/02/12-535/) |

핵심 해석:
- **수사·감정·선거 탐지는 정부가 직접 만들고 계속 고도화한다.** 공공 수요가 커도 민간 판매로 이어지기 어렵다. 선관위가 예산 없이 정부 모델을 무상으로 받아 쓰는 구조가 대표적이다.
- 정부도 탐지 결과를 단독 증거로 쓰지 않고 "수사 참고자료"로만 쓴다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364).
- 국과수 모델 정확도는 요약본끼리 엇갈린다(92% vs 앙상블 97%). 한국 요약본 검증이 "97%는 기사 제목뿐"이라고 확인해 92%를 쓴다.
- 탐지 SW가 혁신제품으로 지정된 사례는 아직 없다(지정되면 3년 수의계약 가능) [조달청](https://pps.go.kr/kor/content.do?key=00648).

### 5.3 국내 플레이어

| 회사·제품 | 모달리티 | 형태·대상 | 현황 | 성능(구분) | 출처 |
|---|---|---|---|---|---|
| 딥브레인AI 딥페이크 탐지 | 영상·이미지·음성 | SaaS·API·온프레미스 / 정부·기업 | 경찰청 SW 1차 개발 협력, 2025.11 API 개방, GS인증 1등급 | 90% 이상·AI 가드 96%(벤더 주장). GS인증은 품질 인증이지 정확도 검증이 아님 | [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366) [디데일리](https://www.ddaily.co.kr/page/view/2025111410120875507) |
| 스틸컷 StealCut | 영상·이미지 | 기업 플랫폼·API / 기업·미디어·로펌 | 2026.8 시드(매쉬업벤처스), TIPS, KTOA 경진대회 대상, AI 혁신조달 대전 최우수상 | 95.2~96%(벤더 주장) | [머니투데이](https://www.mt.co.kr/future/2026/08/11/2026081109014616088) [ZDNet](https://zdnet.co.kr/view/?no=20260918125809) |
| 무하유 GPT킬러 | 글 | 웹·기관 / 대학·공공·채용 | 대학 유통 장악, 표절·AI 보고서 분리 | 98%(벤더 주장) | [아이티데일리](https://www.itdaily.kr/news/articleView.html?idxno=223370) [AI타임스](https://www.aitimes.com/news/articleView.html?idxno=207851) |
| 한컴위드 스피키 | 음성 | 화자인증 / 금융 | 경찰 SW 고도화 참여 | 벤더 발표뿐 | [바이라인](https://byline.network/2026/09/11-703/) |
| 알체라 eKYC | 얼굴 영상 | SDK·API / 금융 본인확인 | 운영 중 | iBeta PAD 통과는 회사 주장, 원문 미확인 | [알체라](https://www.alchera.ai/resource/blog/ekyc-deepfake-detection-identity-verification) |
| 라온시큐어 | 얼굴 이미지 | 백신 앱 내장·API / 소비자 | 2025.1 무료 출시 | 미공개 | [이투데이](https://www.etoday.co.kr/news/view/2439014) |
| 샌즈랩 FakeCheck 2.0 | 얼굴 이미지(영상 가능성) | 무료 웹 / 소비자 | 2025.5 2.0 | 99.33%(300장, 미확인) | [인공지능신문](https://www.aitimes.kr/news/articleView.html?idxno=34963) |
| 누리랩 | 영상·메타데이터 | 통합 시스템 / 공공 | 2025.11 특허 등록, 미출시 | - | [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194) |
| KAIST KaiCatch | 이미지 | Android 앱 / 소비자 | 2022년 이후 정체 | - | [이데일리](https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=02725686628988568) |
| 카카오 kanana·네이버 | (표시용) | 자사 생성물 워터마크 | 외부 콘텐츠 판별 기능 없음 | - | [머니투데이](https://www.mt.co.kr/article/2026012216142218479) |

- **독립 벤치마크로 검증된 국산 탐지 제품은 하나도 없다.** 공개 수치는 모두 벤더나 정부의 자체 발표다.
- 한국인 얼굴 공개 데이터셋은 딥브레인AI의 KoDF(2021)가 마지막이고 갱신판은 미확인이다 [ITWorld](https://www.itworld.co.kr/article/3554516/%EC%98%81%EC%83%81%EC%9D%80-%EB%AC%BC%EB%A1%A0-%EC%9D%B4%EB%AF%B8%EC%A7%80%C2%B7%EC%9D%8C%EC%84%B1%EA%B9%8C%EC%A7%80-%EB%94%A5%EB%B8%8C%EB%A0%88%EC%9D%B8ai-%EB%94%A5%ED%8E%98.html).
- 투자 신호가 약하다. 국내 탐지 전문 스타트업 VC 투자는 스틸컷 시드 외에 확인되지 않았고, 딥브레인AI의 확인 가능한 투자는 2021 Series B까지다 [The VC](https://thevc.kr/deepbrainai/fundings).
- 무하유 카피킬러 캠퍼스 검사 약 85.2만 건(2026.4)은 텍스트 요약본이 [머니투데이](https://www.mt.co.kr/amp/future/2026/05/26/2026052609184984243)를 근거로 적었지만 한국 요약본 검증에서는 재확인되지 않았다(미확인).

### 5.4 대기업·통신사 무료 기능

| 제공자 | 기능 | 합성음(딥보이스) 직접 탐지 | 규모·성능 | 출처 |
|---|---|---|---|---|
| 삼성전자 | 갤럭시 "보이스피싱 의심 알림"(OS 기본, 2025.7) | 근거 없음(통화 문맥 기반) | 사용률 약 84% | [바이라인](https://byline.network/2026/04/27-613/) |
| SK텔레콤 | 에이닷 전화·AI안심차단(망 기반) | 근거 없음(문맥·성문 기반) | 2025년 약 11억 건 차단 | [바이라인](https://byline.network/2026/01/13-583/) |
| KT | AI 보이스피싱 탐지 2.0·후후, 3.0(안심365, 2026.11.4) | 예 | 딥보이스 98%(벤더 주장), 3.0은 판단 근거 제공, 통신사 무관 Android | [디데일리](https://www.ddaily.co.kr/page/view/2025072908585835162) [코리안센터](https://www.koreancenter.or.kr/news/articleView.html?idxno=1436290) |
| LG유플러스 | 익시오 안티딥보이스(온디바이스, 2025.6) | 예 | 98%(벤더 주장), 첫 달 약 5,500건 탐지, 국과수에 무상 제공 | [한경](https://www.hankyung.com/article/202506260996i) [머니투데이](https://www.mt.co.kr/tech/2025/07/23/2025072315221813011) |
| Google(해외) | SynthID Detector, 파트너에 Kakao 포함 | 자사·파트너 워터마크만 | 무료, 영어 | [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/) |

- 실시간 통화 탐지는 **무료 기본 기능으로 이미 포화**됐다. 게다가 Google Play 정책 때문에 신규 소규모 앱은 통화 음성에 사실상 접근할 수 없다 [Engadget](https://www.engadget.com/google-is-banning-third-party-call-recording-apps-from-the-play-store-093201443.html).
- KT 3.0이 판단 근거까지 보여 주면서 "근거를 설명해 주는 탐지"라는 차별점도 줄었다 [코리안센터](https://www.koreancenter.or.kr/news/articleView.html?idxno=1434357).
- 정부가 실제 범죄 음성을 통신사 학습에 지원해, 신규 팀이 "한국어 데이터를 직접 모은다"는 강점도 상대적으로 약해졌다 [바이라인](https://byline.network/2026/02/12-535/).

### 5.5 남은 공백과 진입 장벽

**남은 공백(모두 "빈 시장"이 아니라 "초기 경쟁 단계")**

| 공백 | 왜 비어 있나 | 이미 움직이는 곳 | 출처 |
|---|---|---|---|
| 증거 연속성·설명을 갖춘 한국어 음성 파일 감정 리포트(로펌·보험·노동·민사 분쟁) | 통신사 기능은 실시간 통화 전용, 딥브레인AI는 0~100 확률만, 숭실대 AISRC는 연구용 | 대검·국과수(수사용 내재화), 특수감정인 내세운 포렌식 업체 | [ITWorld](https://www.itworld.co.kr/article/3575761/%EB%94%A5%EB%B8%8C%EB%A0%88%EC%9D%B8ai-saas%ED%98%95-%EB%94%A5%ED%8E%98%EC%9D%B4%ED%81%AC-%ED%83%90%EC%A7%80-%EC%86%94%EB%A3%A8%EC%85%98-%EC%B6%9C%EC%8B%9C%EC%9D%8C%EC%84%B1-%ED%95%A9.html) [K포렌식](https://digitalforensics.co.kr/) |
| 한국 특화 공개 벤치마크(동의 기반 합성 데이터) | KoDF(2021) 이후 확산모델·한국어 TTS를 반영한 공개 벤치마크 없음 | 없음(요약본 기준) | - |
| AI 음악 판별 B2B | 국산 제품 없음, 감사원이 저작권 단체의 AI 확인 부재 지적 | ACRCloud, 음저협 자체 개발 검토 | [주간경향](https://weekly.khan.co.kr/article/202610130600011) [위키트리](https://www.wikitree.co.kr/articles/1137778) |
| 워터마크·C2PA 검증 + 표시 없는 AI 콘텐츠 추정 | 정부 해석상 개인이 워터마크를 지워도 위반 아님 → 표시 없는 AI 콘텐츠가 합법 유통 | Google SynthID Detector(무료, 이미지·영상·오디오) | [다음](https://v.daum.net/v/20260121120209717) |
| 선관위 아이기스 유료 전환 시점의 경쟁 입찰 | 라이선스 만료 후 유료 전환 예정, 다음 피크는 2028.4 총선 | 국과수·KETI | [다음](https://v.daum.net/v/6VGDUSx2ab) |
| 정부 R&D 컨소시엄 참여 | IITP 유통차단·데이터검증 과제 2027년 시작, 경찰 91억 원 과제 | ETRI·KETI·카카오·네이버 등 | [디데일리](https://www.ddaily.co.kr/page/view/2026051314145159743) |

**진입 장벽**
- **공공 수요의 무상 구조**: 정부 모델을 무상으로 나눠 쓰고, 선관위는 전용 예산이 없다. 공공 수요가 매출로 이어지기 어렵다 [다음](https://v.daum.net/v/6VGDUSx2ab).
- **국내 신생 경쟁자의 선점**: 스틸컷이 혁신조달(혁신제품 지정 컨설팅·시범구매)과 로펌·방송사 B2B를 먼저 두드리고 있다 [비석세스](https://besuccess.com/?p=185339).
- **증거능력**: 법정 감정은 국과수 중심이고, 정부도 탐지 결과를 단독 증거로 쓰지 않는다. 국내 대학도 텍스트 탐지 결과를 보조 참고로만 쓰라고 안내한다 [이화여대](https://ewha.libguides.com/GenAI/AIDetection). 교육부·대교협 가이드라인 보도는 미확인이다.
- **학습 데이터의 법적 제약**: 2024.10 개정법으로 허위영상물 소지·시청도 처벌 대상이라 실제 성착취 딥페이크를 학습용으로 모을 수 없다. 얼굴·음성은 민감정보다 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877).
- **공공조달 요건**: GS인증, 보안적합성, 망분리, 납품 실적이 필요하고 영업 주기가 길다.
- **기술 군비경쟁**: 새 생성모델이 계속 나오고 워터마크·메타데이터는 쉽게 지워진다 [ZDNet](https://zdnet.co.kr/view?no=20261020095628).
- **특허**: 앱 개념 전체를 막는 특허는 없다. 딥브레인AI(음성·행동패턴), 누리랩(메타데이터 결합), 스틸컷(5건 출원), 대검(합성음성)의 기법 특허가 있어 FTO 조사가 필요하다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194) [디지털투데이](https://www.digitaltoday.co.kr/en/view/91565/stealcut-deepfake-blocking-ai-security-startup-raises-seed-funding-from-mashup-ventures).
- **규제 수요는 아직 약함**: AI 기본법(2026.1.22 시행)은 표시 의무를 AI 사업자에게 지우고 과태료는 계도기간 동안 유예한다 [뉴시스](https://www.newsis.com/view/NISX20260121_0003485509). "계도 1년 이상·최대 3,000만 원"은 이미지·음성 요약본이 [머니투데이](https://www.mt.co.kr/tech/2025/12/31/2025123009504430416) 등을 근거로 적었으나 한국 요약본 검증에서는 미확인으로 남았다.

**정리**: 한국 시장은 피해는 크지만, 수사·선거·통화·텍스트는 정부·대기업·기존 사업자가 이미 차지했다. 소규모 팀에게 남은 현실적 경로는 "민간 분쟁용 설명가능 감정 리포트 + 공개 벤치마크로 신뢰 확보 + 정부 R&D 컨소시엄·B2B" 조합이며, 이마저도 스틸컷·딥브레인AI와 경쟁해야 한다.


## 6. 특허·데이터 라이선스

> **이 절은 법률 자문이 아니며, 출시 전 변리사의 FTO(실시 가능성) 검토가 필요하다.** FTO는 "내 제품이 남의 특허를 침해하지 않고 팔 수 있는지"를 따지는 조사다. 이번 조사는 특허 청구항 전문을 원문으로 확인하지 못했고(서지 사항만 USPTO 공보·Justia로 확인), 작성자는 변호사·변리사가 아니다.

요지: **"업로드하면 AI인지 판별한다"는 개념 전체를 막는 특허는 발견되지 않았다.** 특허 때문에 포기할 영역은 아니다. 다만 개별 구현 특허가 늘고 있고, 실제로 더 큰 장벽은 **학습 데이터 라이선스**다.

### 6.1 포괄 특허가 있는가

- 딥페이크 탐지·방지 출원은 2018년 이후 급증했다. 국가별 누적은 중국 1,288건, 미국 205건, 한국 151건, 유럽 42건, 일본 34건이고, 2024년 한 해 IP5 출원은 329건이다 [특허뉴스](http://e-patentnews.com/14873). 국내 최다 출원인은 집계마다 다르다(삼성전자·성균관대 대 LG전자) [KISTI ScienceON](https://scienceon.kisti.re.kr/aiq/issue/selectIssueReportView.do?searchIssueRptNo=171&searchDataSectionId=tab_keyword).
- 확인한 등록 특허는 모두 **특정 구현 단위**다(혈류 신호, 점수 결합 방식, 대상자별 모델 등). 개념 자체는 2019년 이전부터 논문(FaceForensics++, FakeCatcher)으로 공개돼 있다.
- 미국에서는 "기존 머신러닝을 새 데이터에 적용한" 수준의 특허는 무효가 될 수 있다는 판례가 있다(Recentive v. Fox, 2025-04) [GT Law](https://www.gtlaw.com/en/insights/2025/4/federal-circuit-machine-learning-patents-ineligible-in-recentive-analytics-inc-v-fox-corp). 그러나 같은 판결은 "모델 자체의 개선"은 특허가 될 수 있다고 열어 뒀다 [Nixon Peabody](https://nixonpeabody.com/insights/alerts/2025/06/24/federal-circuit-limits-patent-eligibility-of-machine-learning-in-recentive-analytics-v-fox). 구조나 학습법을 청구한 특허는 쉽게 무효가 되지 않는다.
- 2025~2026년에는 저화질 탐지, 생성 도구 귀속(어떤 AI로 만들었는지 맞히기), 음성 탐지처럼 **범용 기능에도 등록이 쌓이고 있다** [USPTO 12586419](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586419). "회피가 쉽다"는 낙관은 줄여야 한다.
- 탐지 모델 자체를 둘러싼 침해 소송은 찾지 못했다(미국 법원 기록 PACER는 조회하지 않음). 실제 분쟁은 **출처증명(C2PA)과 얼굴 라이브니스(eKYC)** 쪽에서 일어나고 있다.

### 6.2 주요 특허·분쟁 예시

| 권리 | 권리자 | 내용 | 상태 | 리스크 |
|---|---|---|---|---|
| EP 2 949 070 | KeeeX(프랑스) | 데이터 무결성 검증. OpenAI·Adobe·Truepic·C2PA를 유럽통합특허법원(UPC)에 제소 | 2026-03 항소법원이 일부 국가 관할 부정, 2026-10 파리 본안 심리 시작, 피고 무효 반소, 판결 전 [JUVE Patent](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/) | C2PA 기능을 넣으면 높음 |
| FaceTec 라이브니스 특허 50건 | FaceTec(미국) | 얼굴이 실제 사람인지 확인 | 2026-06 PTAB가 Jumio의 무효 청구 4건 기각, iProov·Jumio 소송 진행 [Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents) | eKYC로 확장 시 높음 |
| US12142083B2 | Pindrop(미국) | 화자·얼굴 딥페이크 + 인식 + 립싱크 점수 결합 | 2024-11-12 등록 [Justia](https://patents.justia.com/patent/12142083) | 영상·음성 교차검증 시 주의 |
| US12412376 등 3건 | Reality Defender(미국) | 가짜 영상 ML 탐지, 오디오 가짜 탐지 | 2025-09~11 등록 [USPTO 공보](https://patentsgazette.uspto.gov/week44/OG/html/1540-1/US12462813-20251104.html) | 청구 범위 미확인 |
| US12475695B2 | Intel(미국) | 대상자별 학습 모델로 특정 인물 사칭 탐지 | 2025-11-18 등록 [USPTO 공보](https://patentsgazette.uspto.gov/week46/OG/html/1540-3/US12475695-20251118.html) | 인물 맞춤 탐지 시 주의 |
| US11687778B2 등 | SUNY(미국) | 혈류 신호(PPG) 맵 + CNN(FakeCatcher 연관) | **미확인** [Google Patents](https://patents.google.com/patent/US11687778) | 논문 방법 그대로 제품화 시 주의 |
| US12586395 등 3건 | 미상(미국) | 도구 귀속, 저화질 탐지, 이중 트랙 음성 탐지 | 2025~2026 [USPTO PDF](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586395) | 범용 기능 영역으로 확산 신호 |
| US12253988 | Originality.ai(캐나다) | 통합 텍스트 검증(AI 탐지는 일부) | 2025-03-18 등록 [Justia](https://patents.justia.com/assignee/originality-ai-inc) | 텍스트 기능 시 확인 필요 |
| 국내 등록(번호 미확인) | 누리랩(한국) | AI + 메타데이터 이상 패턴 | 2025-11 등록 보도 [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194) | 국내 출시 시 확인 필요 |

C2PA의 특허 정책은 요약본끼리 엇갈린다. 출처증명 요약본은 C2PA를 "로열티 프리, 비용은 인증서 수수료뿐"으로 정정했고 [C2PA FAQ](https://www.c2pa.org/faq), 특허 요약본은 특허 정책을 미확인으로 남겼다. 어느 쪽이든 **KeeeX는 C2PA 회원이 아니므로 로열티 프리 정책으로도 KeeeX 리스크는 사라지지 않는다**(추론). 중국 출원이 압도적이고 주요 출원인이 핑안·바이두·텐센트이므로, 중국 진출 시 FTO 범위를 넓혀야 한다 [특허뉴스](http://e-patentnews.com/14873).

### 6.3 데이터셋·모델 라이선스

탐지 모델은 학습 데이터가 생명이다. 그런데 **가장 유명한 벤치마크 데이터 상당수가 상업적 이용을 금지한다.** 연구용으로 성능을 낸 모델을 그대로 앱에 넣으면 라이선스 위반이 될 수 있다.

| 자원 | 종류 | 라이선스 | 상업 이용 | 근거 |
|---|---|---|---|---|
| GenImage | AI 이미지 데이터셋 | CC BY-NC-SA 4.0 + 추가 약관 | **불가**(파생물 포함) | [GenImage](https://genimage-dataset.github.io) |
| FaceForensics++ | 딥페이크 영상 데이터셋 | 비상업 연구·교육 전용 | **불가**(독립 재확인 못함) | [TUM ToS](https://kaldir.vc.in.tum.de/faceforensics_tos.pdf) |
| DeepfakeBench | 탐지 벤치마크 | CC BY-NC 4.0 | **불가** | [GitHub](https://github.com/sclbd/deepfakebench) |
| DFDC, Celeb-DF | 딥페이크 영상 데이터셋 | 약관 원문 미확인 | 미확인 | - |
| ASVspoof 2019/5 | 가짜 음성 데이터셋 | ODC-By 1.0 | **가능**(출처 표시) | [ASVspoof 2019 논문](https://arxiv.org/pdf/1911.01601) |
| Stanford GPIC | 실사진 1억 장 | 상업 이용 가능 | **가능** | [AI Weekly](https://aiweekly.co/alerts/stanfords-gpic-ships-100m-commercially-usable-training-images) |
| TrueMedia 공개 코드 | 다중 모달 탐지 코드 | MIT | **가능**. 단 학습된 가중치는 공개 보류 | [TrueMedia](https://www.truemedia.org/post/open-source-release) |
| TrueMedia GenConViT | 영상 탐지 구성요소 | GPL-3.0 | 조건부(배포 형태에 따라 소스 공개 의무) | [GitHub](https://github.com/truemediaorg/GenConViT) |
| Google SynthID Text | 텍스트 워터마크 구현 | HF Transformers에 오픈소스 구현 | 특허 여부 미확인 | [Google](https://ai.google.dev/responsible/docs/safeguards/synthid?hl=en) |

추가로 확인할 것:
- **개인정보·초상권:** 데이터셋 속 얼굴·음성은 개인정보다. 수사용으로 쓰면 데이터 출처의 적법성이 증거능력 다툼 대상이 될 수 있다(추론).
- **실전 범죄 데이터:** 한국은 허위영상물 소지·시청까지 처벌하므로 실제 성착취 딥페이크를 학습용으로 모으기 어렵다 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877).
- **약관:** OpenAI는 워터마크를 역공학하려는 반복 질의를 금지한다 [OpenAI](https://openai.com/index/advancing-content-provenance).
- **상표:** "AI Detector"처럼 기능을 설명하는 이름은 등록이 어렵고 기존 브랜드와 충돌할 수 있다. 9류·42류 선행 조사가 필요하다(미확인(사전 지식)).

### 6.4 판단

| 질문 | 답 |
|---|---|
| 이미 포괄 특허가 있어 포기해야 하나? | **아니다.** 개념 전체를 막는 특허는 발견되지 않았다 |
| 그럼 마음대로 만들어도 되나? | **아니다.** 구현마다 회피 설계와 FTO가 필요하다. 범용 기능 영역에도 특허가 늘고 있다 |
| 가장 위험한 확장 방향은? | C2PA 서명·검증(KeeeX 소송), 얼굴 라이브니스·eKYC(FaceTec 등). 이쪽으로 넓히면 특허 리스크가 크게 오른다 |
| 실제 최대 장벽은? | **학습 데이터.** 대표 벤치마크가 비상업 전용이다. 상업 가능 데이터(ASVspoof, Stanford GPIC)에 최신 생성기로 직접 합성한 데이터를 더하는 방식이 필요하다 |
| 할 만한 방어 수단은? | 자체 구현(증거 패키징, 모달 간 교차검증 방식 등)을 국내에 방어적으로 출원하면 투자 유치·분쟁 협상에 도움이 된다(추론) |

특허 측면의 레드오션 판정은 **"부분적"**이다. 특허로 막혀 포기할 정도는 아니지만, 쉽게 피해 갈 수 있다고 낙관할 수도 없다. **다시 강조한다. 이 절은 법률 자문이 아니며, 출시 전 변리사의 FTO(실시 가능성) 검토가 필요하다.**


## 7. 시장 규모·투자·비즈니스 모델

요지: **돈은 기업용 실시간 사칭 방어(콜센터·화상회의·채용)와 텍스트 탐지(교육)로 흐르고 있다.** 소비자용 "AI 판별 앱"으로 의미 있는 매출을 낸 사례는 확인되지 않는다. 2026년에는 인수·투자로 통합이 시작됐고, 탐지는 단독 제품보다 큰 플랫폼의 한 기능으로 흡수되는 중이다.

### 7.1 시장 규모 추정치

모두 판매용 시장조사 보고서의 추정치라 신뢰도는 낮다. 정의(탐지 전용인지, 신원확인 전체인지)에 따라 수치가 크게 다르다.

| 기관 | 기준연도 규모 | 전망 | 연 성장률 | 근거 |
|---|---|---|---|---|
| Meticulous Research | 2025년 7.1억 달러(2026년 9.9억 달러) | 2036년 94.4억 달러 | 25.3% | [Meticulous](https://www.meticulousresearch.com/product/deepfake-detection-market-6944) |
| SNS Insider | 2025년 9.19억 달러 | 2035년 121억 달러 | 미기재 | [SNS Insider](https://www.snsinsider.com/reports/deepfake-detection-market-11090) |
| Astute Analytica | 2025년 7.0억 달러 | 2035년 90억 달러 | 미기재 | [Astute](https://www.astuteanalytica.com/industry-report/deepfake-detection-market) |
| LP Information | 2024년 1.98억 달러 | - | - | 이상치·정의 다름(미확인) |
| MRFR | 2024년 17.32억 달러 | - | - | 이상치·정의 다름(미확인) |

탐지 전용 기준으로는 **2025년 약 7억~10억 달러, 연 25~30% 성장**으로 모인다. 수치가 10배 넘게 벌어지는 보고서는 정의가 다른 시장을 섞은 결과다.

참고로 피해 규모 전망은 훨씬 크다. Deloitte는 미국 생성형 AI 사기 손실이 2023년 123억 달러에서 2027년 400억 달러로 늘 수 있다고 본다(시나리오 전망) [Deloitte](https://www.deloitte.com/us/en/insights/industry/financial-services/deepfake-banking-fraud-risk-on-the-rise.html). 한국 보이스피싱 피해액은 2024년 8,545억 원에서 2025년 1조 2,578억 원으로 늘었지만, 딥보이스 사건만 따로 센 통계는 없다 [아이뉴스24](https://www.inews24.com/view/2008688).

그런데 **위협 인식이 지출로 바로 이어지지는 않는다.** 보안 리더의 약 3/4이 딥페이크 공격을 겪었거나 의심했지만 전용 방어책을 갖춘 곳은 10%였다(벤더 조사) [HelpNetSecurity](https://helpnetsecurity.com/2026/09/29/pindrop-enterprise-deepfake-attacks-report). 사이버보험사 Coalition은 청구 건의 98%가 고급 AI와 무관하다고 밝혔다 [CyberScoop](https://cyberscoop.com/?p=87093).

### 7.2 최근 투자·인수

| 시기 | 회사 | 거래 | 금액 | 의미 | 근거 |
|---|---|---|---|---|---|
| 2024-07 | Pindrop(음성) | 투자 | 지분 2.183억 달러 + 부채 1억 달러 | 콜센터 음성 강자, ARR 1억 달러 돌파(벤더 주장) | [HelpNetSecurity](https://www.helpnetsecurity.com/2024/07/18/pindrop-financing-100-million/) |
| 2024-10 | Reality Defender | Series A | 3,300만 달러 | 기업용 멀티모달 API | [DCVC](https://dcvc.com/press-releases/reality-defender-expands-series-a-to-33-million-to-enhance-ai-detection-capabilities) |
| 2025-03 | GetReal Security | Series A | 1,750만 달러(In-Q-Tel 참여) | 포렌식·정부 | [SecurityWeek](https://www.securityweek.com/getreal-security-raises-17-5-million-to-tackle-gen-ai-threats/) |
| 2025-11 | Doppel | Series C | 7,000만 달러, 기업가치 6억 달러 이상 | 사칭 대응 플랫폼 | [SecurityWeek](https://www.securityweek.com/doppel-raises-70-million-at-600-million-valuation/) |
| 2025-12 | Resemble AI | 투자 | 1,300만 달러 | 음성 생성+탐지 | [SiliconANGLE](https://siliconangle.com/2025/12/08/resemble-ai-hauls-13m-different-approach-deepfake-detection/) |
| 2026-03 | Neuramancer | 프리시드 | €1.7M | 신규 진입자 | [Tech.eu](https://tech.eu/2026/03/12/neuramancer-lands-eur17m-pre-seed-to-scale-deepfake-detection-tools) |
| 2026-06-23 | GPTZero → Superhuman | **인수** | 비공개(8,800만 달러 이상은 매체 추정) | 텍스트 탐지가 생산성 앱 기능으로 | [AI Weekly](https://aiweekly.co/alerts/superhuman-acquires-gptzero-to-add-ai-authenticity-layer) |
| 2026-07 | Pangram | 투자 | 900만 달러 | 텍스트 탐지 | [TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/) |
| 2026-07 | Sensity | EU 보조금+지분 | €4.9M | 포렌식 리포트 | [BiometricUpdate](https://www.biometricupdate.com/202607/sensity-ai-gets-eic-funding-for-forensics-focused-deepfake-detection-models) |
| 2026-08-03 | Clarity → Deel | **인수** | 4,500만~5,000만 달러(현금+주식). Calcalist는 4,000만~5,000만 달러로 보도 | 채용 신원확인 기능으로 | [TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/), [Calcalist](https://calcalistech.com/ctechnews/article/bkeyex0sgl) |
| 2026-09-10 | Reality Defender ← KPMG | **소수지분 인수** | 비공개 | 컨설팅사 채널로 흡수 | [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html) |
| 2026-09 | Modulate | 투자 | 2,500만 달러(누적 6,000만 달러) | 음성·AI 음악 탐지 | [TechCrunch](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/) |
| 2026-08 | 스틸컷(한국) | 시드(매쉬업벤처스) | 요약본에 없음 | 국내 신규 진입자 | [머니투데이](https://www.mt.co.kr/future/2026/08/11/2026081109014616088) |

읽는 법:
- 순수 탐지 스타트업 한 곳의 조달액은 대개 **1,000만~3,500만 달러**다. 기업 실시간 방어 분야는 수천만~억 달러 단위 자본 경쟁이다.
- 엑시트는 대부분 **큰 플랫폼에 인수**되는 형태다. Clarity(누적 투자 1,600만 달러)가 기준점이지만, 대금에 주식이 섞여 있어 "투자금의 3배를 현금 회수"로 읽으면 과장이다 [Dealroom](https://dealroom.co/news/142736-deel-acquires-clarity-to-strengthen-identity-verification-surpasses-1-5b/).
- Gartner는 2026-06 딥페이크 탐지를 독립 카테고리로 만들었다 [BiometricUpdate](https://www.biometricupdate.com/202609/kpmg-investment-in-reality-defender-backs-hiring-spree-to-fight-deepfakes). 시장이 "통합 단계"에 들어섰다는 신호다.

### 7.3 누가 돈을 내는가

| 세그먼트 | 지불 의사 | 대표 사업자 | 소규모 팀 진입 가능성 | 근거 |
|---|---|---|---|---|
| 콜센터·금융(음성 사칭) | **높음.** 규모 있는 매출이 확인된 유일한 멀티모달 분야 | Pindrop(ARR 1억 달러 이상, 2025년부터 흑자, 벤더 주장) | 낮음(자본·채널 격차) | [BiometricUpdate](https://www.biometricupdate.com/202504/pindrop-surpasses-100m-in-annual-recurring-revenue-kicks-off-bu-podcast), [Mergermarket](https://ionanalytics.com/insights/mergermarket/pindrop-could-step-up-acquisitions-in-agentic-security-as-its-deepfake-detection-takes-off-ceo/) |
| 교육(AI 글 탐지) | **높음.** 기관 번들로 판매 | Turnitin(AI 탐지 매출 별도 비공개), GPTZero(사용자 1,900만 명·ARR 3,000만 달러, 벤더 주장) | 낮음(이미 인수·통합) | [Sacra](https://sacra.com/c/turnitin/), [CryptoBriefing](https://cryptobriefing.com/superhuman-acquires-gptzero-ai-detector/) |
| 기업 보안(화상회의·사칭) | 중간~높음 | Reality Defender, GetReal, Doppel, imper.ai | 낮음 | [SecurityWeek](https://www.securityweek.com/imper-ai-emerges-from-stealth-mode-with-28-million-in-funding/) |
| 채용·HR | 중간(성장 중) | Clarity(Deel 인수) | 플러그인·인수형으로 가능 | Gartner: 2028년 지원자 프로필 4개 중 1개가 가짜일 수 있음(전망) [Allwork](https://allwork.space/2025/04/ai-deepfake-scammers-infiltrating-the-hiring-processes-at-alarming-rates-gartner-reports/) |
| 플랫폼·국방 | 중간 | Hive(DIU 240만 달러) | 낮음 | [BusinessWire](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats) |
| 보험·법무·언론(감정 리포트) | 중간. Coalition이 딥페이크 특약에 포렌식 분석·서면 보고서를 넣음 | Sensity, GetReal Inspect | **상대적으로 가능** | [Reinsurance News](https://www.reinsurancene.ws/coalition-enhances-cyber-product-with-addition-of-deepfake-response-endorsement) |
| 한국 수사기관(B2G) | 있지만 국가 시스템과 경쟁 | 경찰청 91억 원 과제, 국과수 모델 | 낮음. 완료 후 전 수사기관 공동 시스템 계획 | [korea.kr](https://www.korea.kr/news/policyNewsView.do?newsId=148973649) |
| 한국 선관위 | **사실상 없음.** 딥페이크 전용 예산 '전무', 정부 모델을 무상으로 받아 씀. 라이선스 만료 후 유료 전환 예정 | 국과수 아이기스 | 2028년 4월 총선 전 입찰 여지 | [다음](https://v.daum.net/v/6VGDUSx2ab) |
| 일반 소비자 | **낮음.** 무료 대체재가 넘침 | Google·YouTube·Hiya(무료), Norton·McAfee(유료 보안 번들, 영어만) | 낮음 | [SecurityBrief](https://securitybrief.co.uk/story/norton-rolls-out-ai-deepfake-scam-protection-for-intel-pcs) |

가격 기준선도 있다. Reality Defender는 무료 월 50회, 유료 월 399달러에 1,000회(약 0.4달러/회)를 공개했다 [Intercom 가격](https://intercom.help/reality-defender/en/articles/12831411-managing-your-plan-billing). 소규모 팀이 범용 API를 팔려면 이 가격과 경쟁해야 한다.

### 7.4 소비자 앱 모델의 현실

사용자가 처음 구상한 "의심 파일을 넣으면 AI인지 알려 주는 앱"은 사업으로서 가장 어려운 형태다.

| 문제 | 근거 |
|---|---|
| 무료 대체재 | Google SynthID 포털·Search·Chrome·Gemini, YouTube 초상 탐지(무료), Hiya Chrome 확장(무료), Reality Defender 무료 티어 [SocialMediaToday](https://www.socialmediatoday.com/news/youtube-expands-likeness-detection-to-all-users-over-18/820440/), [Engadget](https://www.engadget.com/ai/a-new-chrome-extension-can-reliably-detect-ai-generated-voices-130059842.html) |
| 앱스토어 평판 | 소비자 탐지 앱은 작동하지 않거나 사기성 리뷰가 많다는 지적 [Copyleaks 블로그](https://copyleaks.com/blog/ai-detector-apps-arent-what-they-claim) |
| 운영비 | 무료 비영리 TrueMedia는 높은 운영비로 2025-01 독자 운영을 접고 Georgetown 클로즈드 베타로만 남음 [TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia), [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/) |
| 매출 공개 없음 | AI or Not 등 소비자 앱의 재무는 미확인. 멀티모달 스타트업 Sensity도 2026년 ARR 400만 달러 이상이 목표(벤더 주장) [Simplify](https://simplify.jobs/c/Sensity) |
| 오탐 책임 | 소비자 도구 오탐률이 최대 40%(NewsGuard). 일반인이 결과를 믿고 남을 고발하면 분쟁이 생김 [NewsGuard](https://www.newsguardtech.com/?p=33448) |
| 기능 흡수 | GPTZero는 Superhuman에, Clarity는 Deel에 흡수됨. 탐지는 독립 앱보다 다른 서비스의 기능이 되는 흐름 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection) |

**결론:** 소비자 앱은 레드오션이고 수익화가 어렵다. 텍스트 분야만 예외적으로 소비자 규모를 만들었지만(GPTZero) 결국 인수로 끝났다. 현실적인 비즈니스 모델은 **좁은 B2B 버티컬(보험·법무·언론 감정 리포트, 한국어 보이스피싱 음성, 채용 신원확인)**이고, 출구는 플랫폼 인수형이다. 소비자 앱은 사업의 본체가 아니라 인지도와 데이터를 모으는 입구로만 의미가 있다.


## 8. 경쟁력 종합 판단

### 8.1 세그먼트 매트릭스

| 세그먼트 | 경쟁 강도 | 기회 | 소규모 팀 적합도 | 판정 |
|---|---|---|---|---|
| 범용 소비자 판별 앱(4매체 통합) | 매우 높음(빅테크 무료·보안 번들) | 낮음. 유료화 어려움 | 낮음 | **포기** |
| "유명 AI로 만들었나" 워터마크 확인 | 매우 높음(Google·OpenAI 무료, 캘리포니아법 의무화) | 거의 없음 | 낮음 | **포기** |
| 영어 글 탐지 | 매우 높음(Turnitin, Superhuman+GPTZero) | 낮음 | 낮음 | **포기** |
| 한국어 글 탐지 | 높음(무하유 장악, Turnitin 확장 중) | 낮음. 공백은 시한부 | 낮음 | **포기** |
| AI 음악 판별 B2B | 높음(Deezer·Modulate·IRCAM) | 국내 초기 시장, 수요 주체 방향 불확실 | 낮음~중간 | 보류 |
| 한국 실시간 통화 보이스피싱 탐지 | 매우 높음(삼성·통신3사 무료) | 없음. Play 정책으로 통화 접근 차단 | 매우 낮음 | **포기** |
| 콜센터·화상회의 기업 보안 | 매우 높음(Pindrop·Reality Defender) | 있으나 자본 경쟁 | 낮음 | **포기** |
| 한국 수사·선거 B2G | 높음(정부 자체 개발·무상 배포) | 2028 총선 전 입찰, R&D 컨소시엄 정도 | 낮음 | 부수적 참여만 |
| 민간 분쟁용 설명형 감정 리포트(음성·영상·이미지) | 중간(스틸컷·딥브레인AI·포렌식 업체) | 있음. 보험 특약에 포렌식 보고서 포함 | **중간** | **노려볼 만함** |
| 한국 특화 공개 벤치마크 | 낮음(KoDF 2021 이후 없음) | 신뢰·인지도 확보 수단 | **높음** | **노려볼 만함(수익 아님)** |
| 워터마크·C2PA·탐지 통합 검증 리포트 | 중간(Google 무료, 대형사 흡수 가능) | 생태계가 쪼개져 있는 동안 | 중간 | **조건부** |
| 소규모 생성 AI 업체용 검증도구(SB 1000) | 낮음~중간 | 미국 규제 수요 | 중간 | **조건부(해외)** |

근거: 2~7절. 핵심 출처는 [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857), [Morgan Lewis](https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative), [Reinsurance News](https://www.reinsurancene.ws/coalition-enhances-cyber-product-with-addition-of-deepfake-response-endorsement), [다음](https://v.daum.net/v/6VGDUSx2ab).

### 8.2 포기해야 할 영역

| 영역 | 포기 이유 |
|---|---|
| 범용 "AI 확률" 소비자 앱 | 무료 대체재(Google SynthID·Hive 확장·Reality Defender 무료 티어)가 있고, 비영리 TrueMedia도 운영비로 독자 운영을 접었다 [TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia). 오탐 최대 40%로 신뢰를 얻기 어렵다 [NewsGuard](https://www.newsguardtech.com/?p=33448) |
| 워터마크 확인 앱 | 생성사가 법적으로 무료 검증도구를 제공해야 하고, 빅테크 검색·브라우저에 이미 들어갔다 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/) |
| 글(영어·한국어) | 유통이 Turnitin·Superhuman에 묶였고, 한국어는 무하유가 대학을 장악했다. 교육 시장은 "작성 과정 증명"으로 옮겨 가는 중이다 [BusinessWire](https://www.businesswire.com/news/home/20260623083788/en/Superhuman-to-Acquire-GPTZero-AI-Authenticity-Platform) |
| 실시간 통화 탐지 | 삼성(사용률 약 84%)·통신3사가 무료, 정부가 범죄 음성 데이터를 통신사에 지원, Google Play가 통화 접근을 막는다 [바이라인](https://byline.network/2026/02/12-535/) [Engadget](https://www.engadget.com/google-is-banning-third-party-call-recording-apps-from-the-play-store-093201443.html) |
| 수사기관용 감정 시스템 | 경찰 91억 원·대검 86억 원·IITP 300억 원 국책 과제로 정부가 직접 만든다. 선관위는 예산이 "전무" [korea.kr](https://www.korea.kr/news/policyNewsView.do?newsId=148973649) |
| 기업 실시간 사칭 방어 | Pindrop(ARR 1억 달러 이상, 벤더 주장) 등과 수천만~억 달러 단위 자본 경쟁 [BiometricUpdate](https://www.biometricupdate.com/202504/pindrop-surpasses-100m-in-annual-recurring-revenue-kicks-off-bu-podcast) |
| "범죄까지 잡는 범용 정밀 모델" 약속 | 세계 어느 기업·정부도 독립 평가로 입증하지 못했다. 약속하면 오탐·미탐 책임만 커진다 (4절) |

### 8.3 노려볼 만한 포지셔닝

세 가지 모두 "범죄를 잡는 앱"이 아니라 **"사람이 근거를 갖고 더 빨리 판단하도록 돕는 도구"**다. 이것이 현재 기술로 정직하게 약속할 수 있는 최대치다 (4.5절).

#### 포지셔닝 A: 민간 분쟁용 한국어 설명형 감정 리포트 (최우선)

| 항목 | 내용 |
|---|---|
| 타깃 고객 | 로펌·보험사(보험 사기 조사)·노무법인·언론사 팩트체크팀. 개인 의뢰인은 이들을 통해 간접 확보 |
| 해결할 문제 | "이 녹취·영상·사진이 조작됐다"는 주장이 나왔을 때, 국과수 감정은 수사용이고 오래 걸린다. 통신사 기능은 실시간 통화 전용, 딥브레인AI는 0~100 확률만 준다 [ITWorld](https://www.itworld.co.kr/article/3575761/%EB%94%A5%EB%B8%8C%EB%A0%88%EC%9D%B8ai-saas%ED%98%95-%EB%94%A5%ED%8E%98%EC%9D%B4%ED%81%AC-%ED%83%90%EC%A7%80-%EC%86%94%EB%A3%A8%EC%85%98-%EC%B6%9C%EC%8B%9C%EC%9D%8C%EC%84%B1-%ED%95%A9.html) |
| 차별점 | ① 점수가 아니라 근거(메타데이터, 편집 흔적, 워터마크 확인, 탐지 결과, 원본 여부) ② "진짜/가짜/판정 불가" 3단 ③ 파일 해시·처리 이력·모델 버전 기록 ④ 공개 오류율 |
| 기술·데이터 | 오픈소스 탐지 코드(TrueMedia, MIT) + 상용 API 앙상블로 시작 [TrueMedia](https://www.truemedia.org/post/open-source-release). 음성은 ASVspoof(ODC-By)에 최신 한국어 TTS로 직접 합성한 데이터를 더함 [ASVspoof](https://arxiv.org/pdf/1911.01601). 실사진은 Stanford GPIC [AI Weekly](https://aiweekly.co/alerts/stanfords-gpic-ships-100m-commercially-usable-training-images) |
| 수익 모델 | 건당 감정 리포트 요금 + 로펌·보험사 월 구독. 가격 기준선은 Reality Defender API 약 0.4달러/회지만, 리포트는 전문가 검토가 붙어 건당 단가가 높다(단가 근거는 요약본에 없음) |
| 주요 경쟁자 | 스틸컷(로펌·방송사 B2B 선점) [비석세스](https://besuccess.com/?p=185339), 딥브레인AI, 특수감정인 포렌식 업체 [K포렌식](https://digitalforensics.co.kr/), 해외 Sensity·GetReal |
| 리스크 | 오탐 시 손해배상·명예훼손 분쟁, 법원이 증거로 안 받아 줄 가능성(Rule 707은 빨라야 2029-12) [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence), 김수현 사건처럼 원본이 없으면 판정 불가 |
| 첫 3개월 MVP | 음성 파일 1종에 집중. 업로드 → 메타데이터·재인코딩 흔적·SynthID 확인·탐지 앙상블 → PDF 리포트(3단 판정, 근거, 해시). 로펌·보험사 3~5곳과 무료 파일럿, 실제 사건 파일로 오탐·미탐 기록 |

#### 포지셔닝 B: 한국 특화 공개 벤치마크 + 독립 검증

| 항목 | 내용 |
|---|---|
| 타깃 고객 | 국내 탐지 업체, 공공 발주처(경찰·선관위·IITP 과제), 연구자, 언론 |
| 해결할 문제 | 국산 탐지 제품 중 독립 벤치마크로 검증된 것이 하나도 없다. 한국인 얼굴 공개 데이터는 KoDF(2021)가 마지막이다 (5.3절) |
| 차별점 | 확산모델·한국어 TTS를 반영한 동의 기반 데이터, 분기마다 최신 생성기 추가, 상용·공공 모델 성적 공개 |
| 기술·데이터 | 동의받은 참여자 촬영·녹음 + 상업 이용 가능한 생성기로 직접 합성. 실제 범죄물은 쓰지 않음. 텍스트는 KatFish(ACL 2025)가 이미 있어 중복 피함 [ACL Anthology](https://aclanthology.org/2025.acl-long.1030) |
| 수익 모델 | 벤치마크 자체는 공개(인지도·신뢰 확보). 매출은 기업용 비공개 평가 서비스, 정부 R&D 컨소시엄 참여(IITP 유통차단·데이터검증 과제 2027년 시작) [디데일리](https://www.ddaily.co.kr/page/view/2026051314145159743) |
| 주요 경쟁자 | 직접 경쟁자는 요약본상 없음. ETRI·KETI·대학이 정부 과제로 만들 가능성 |
| 리스크 | 단독 매출이 작음. 데이터 참여자 초상권·개인정보 동의 관리, 벤치마크 결과에 대한 업체 반발 |
| 첫 3개월 MVP | 이미지·음성 2개 모달리티, 최신 생성기 5~10종, 수천 건 규모 v0.1 공개. 오픈소스 탐지기와 공개 API 3~5종 성적표 발표 |

#### 포지셔닝 C: 워터마크·출처표식·탐지를 한 번에 보는 통합 검증 API (조건부)

| 항목 | 내용 |
|---|---|
| 타깃 고객 | 국내 언론사·플랫폼 운영자, 미국 캘리포니아 SB 1000 대상인 소규모 생성 AI 업체(화이트라벨 검증도구) |
| 해결할 문제 | SynthID·Meta·Microsoft·C2PA·Apple 표식이 서로 호환되지 않는다 [arXiv 2602.18681](https://arxiv.org/abs/2602.18681). 표식이 없거나 지워진 콘텐츠는 아무도 판정하지 않는다 |
| 차별점 | 여러 표식 판독 + 표식 없을 때 사후 탐지 + "원래 없음/지워짐" 구분을 한 리포트로. 한국어 UI |
| 기술·데이터 | 공개 표식 판독 도구 연동, 사후 탐지는 포지셔닝 A 엔진 재사용. 제거 흔적 탐지는 연구 단계(프리프린트) [arXiv 2605.09203](https://arxiv.org/pdf/2605.09203) |
| 수익 모델 | API 종량제·월 구독. SB 1000은 "자격 있는 제3자 검증도구"로 의무 이행을 허용한다 [Latham](https://www.lw.com/en/insights/newest-slate-of-ai-laws-keeps-california-at-the-forefront-of-us-regulation) |
| 주요 경쟁자 | Google SynthID Detector·기업용 API(무료·프리뷰), Adobe Content Authenticity, Reality Defender |
| 리스크 | EU 상호운용성 기한(2027-02-02) 뒤 대형사가 직접 통합하면 흡수됨. C2PA 영역은 KeeeX 특허 소송 중 [JUVE Patent](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/). OpenAI 약관은 워터마크 역공학 질의 금지 |
| 첫 3개월 MVP | 별도 제품으로 만들지 말고 포지셔닝 A 리포트에 "표식 확인" 항목으로 넣어 수요를 확인. C2PA 서명 기능은 넣지 않고 판독만, 그것도 FTO 뒤에 |

### 8.4 종합

- **우선순위: A(본업) → B(신뢰 확보 수단, A와 병행) → C(A에 기능으로 흡수).**
- 세 포지셔닝 모두 경쟁자가 있고 시장이 작다. "빈 시장"이 아니라 **"초기 경쟁 단계의 좁은 시장"**이다. 스틸컷이 같은 방향(로펌·혁신조달)을 먼저 두드리고 있다 [머니투데이](https://www.mt.co.kr/future/2026/08/11/2026081109014616088).
- 현실적 출구는 대형 플랫폼 인수형이다. Clarity(Deel 인수, 4,500만~5,000만 달러, 현금+주식)가 기준점이지만 과장해 읽으면 안 된다 [TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/).


## 9. 리스크와 주의사항

| 리스크 | 무엇이 문제인가 | 대응 |
|---|---|---|
| 오탐 책임 | 진짜를 가짜로 판정하면 명예훼손·부당 고발·소송으로 이어진다. 소비자 도구 오탐은 최대 40%(독립 평가, 표본 작음) [NewsGuard](https://www.newsguardtech.com/?p=33448). 진짜 참상 사진이 조작으로 판정된 사례도 있다 [PhotoWorkout](https://www.photoworkout.com/?p=222434) | "판정 불가" 출력, 오류율 공개, 단독 증거로 쓰지 말라는 고지, 전문가 검토 |
| 거짓말쟁이의 배당 | 탐지기가 있으면 진짜 증거도 "AI로 만든 것"이라고 우길 수 있다. 국과수 "판정 불가"를 한쪽이 "완승"으로 선전한 사례 [한국경제](https://www.hankyung.com/article/2025121553117) | 판정 불가 사유(원본 아님, 잡음 등)를 리포트에 명확히 적기 |
| 우회 | 캡처·재압축·해상도 축소만으로 흔적이 사라진다 [Reuters Institute](https://reutersinstitute.politics.ox.ac.uk/news/spotting-deepfakes-year-elections-how-ai-detection-tools-work-and-where-they-fail). 탐지기 공격(TIGA)은 우회율 78%를 유지했다 [TIGA](https://arxiv.org/pdf/2604.09706v1). 워터마크도 제거 공격에 뚫렸다(SynthID-Image 100% 제거) [arXiv 2608.10166](https://arxiv.org/pdf/2608.10166) | 탐지 하나에 의존하지 않고 메타데이터·원본 확보·출처 관리와 묶기 |
| 생성기와의 군비경쟁 | 새 생성기가 나오면 성능이 급락한다(최신 영상 94.3→48.2, 독립 평가) [DF26](https://arxiv.org/pdf/2609.07369). 재학습하면 회복되지만 비용이 계속 든다. TrueMedia도 운영비로 독자 운영을 접었다 [TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia) | 분기별 재학습·재평가 예산을 처음부터 사업 계획에 넣기. 도메인을 좁혀 비용 통제 |
| 학습 데이터의 법적 문제 | 허위영상물은 소지·시청만으로 처벌(최고 3년)되어 실제 성착취 딥페이크를 학습용으로 모을 수 없다 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877). 얼굴·음성은 민감정보다. GenImage·FaceForensics++·DeepfakeBench는 상업 이용 금지 [GenImage](https://genimage-dataset.github.io) [DeepfakeBench](https://github.com/sclbd/deepfakebench) | 성범죄 영역은 다루지 않거나 수사기관 협력으로만. 동의 기반 자체 합성 데이터 + 상업 가능 데이터(ASVspoof, GPIC). 데이터 출처 기록 |
| 법적 책임·증거능력 | 법정 감정은 국과수 중심이고 정부도 탐지 결과를 단독 증거로 쓰지 않는다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364). 미국 AI 증거 규칙(Rule 707)은 빨라야 2029-12 [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence). 판례도 탐지 점수가 아니라 비교 증거로 판단했다 [Volokh](https://reason.com/volokh/2025/09/25/court-throws-out-case-after-finding-plaintiffs-submitted-deepfake-videos-and-altered-images/) | 약관에 책임 한도 명시, 전문가 배상책임보험 검토, "참고자료" 위치 고수 |
| 특허 | 개념 특허는 없지만 구현 특허가 쌓이는 중. C2PA(KeeeX)·라이브니스(FaceTec)는 실제 분쟁 중 [Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents) | 출시 전 변리사 FTO. 이 보고서는 법률 자문이 아니다 |
| 빅테크 무료화 | Google SynthID Detector가 2026-10 전 세계 무료 공개, Search·Chrome·Gemini·YouTube에 기본 탑재. 캘리포니아법은 생성사에 무료 검증도구를 의무화 [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/) [MoFo](https://www.mofo.com/resources/insights/261001-california-revamps-ai-transparency-requirements) | 빅테크가 하지 않는 것(표식 없는 콘텐츠, 설명형 리포트, 한국어 B2B 서비스)에만 집중 |
| 개인정보 | 의뢰 파일에 제3자 얼굴·음성이 담긴다. SB 1000 검증도구는 개인정보를 동의 없이 내보내면 안 된다 [Sheppard](https://www.sheppard.com/insights/blogs/california-enacts-ai-spokespeople-chatbots-and-content-disclosures-laws) | 파일 보관 기간 최소화, 국내 처리, 학습 활용은 별도 동의 |

**가장 큰 함정:** "범죄까지 잡는다"는 마케팅이다. 독립 평가로 입증할 수 없는 약속은 오탐 한 건으로 회사를 무너뜨릴 수 있다. 성능은 독립 평가 수치로만 말하라.


## 10. 권장 다음 단계

포지셔닝 A(민간 분쟁용 설명형 감정 리포트)로 간다는 전제의 실행 항목이다. 범용 소비자 앱을 고집한다면 1번에서 멈추고 포기하는 것이 맞다.

| 순서 | 할 일 | 목적·완료 기준 | 기간(제안) |
|---|---|---|---|
| 1 | **방향 결정:** 범용 소비자 앱을 접고 B2B 감정 리포트로 갈지 결정 | 0.2절 조건 5개를 받아들일 수 있는지 팀 합의 | 1주 |
| 2 | **고객 인터뷰 10곳 이상:** 로펌·보험사(사기조사)·노무법인·언론 팩트체크팀 | "건당 얼마를 내겠나", "어떤 파일(음성/영상/사진)이 가장 많나", "리포트에 무엇이 있어야 쓰나" 확인. 유료 의향 3곳 이상이면 진행 | 3~4주 |
| 3 | **변리사 FTO 1차 검토** | 딥브레인AI·스틸컷·대검·누리랩·Pindrop 특허와 겹치는지 확인. C2PA·라이브니스는 범위에서 제외 [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194) | 4~6주(병행) |
| 4 | **데이터 라이선스 정리** | 상업 가능 데이터(ASVspoof, Stanford GPIC, TrueMedia MIT 코드) 목록화. 비상업 데이터(GenImage·FaceForensics++·DeepfakeBench)는 제품 학습에서 제외. 성범죄물은 다루지 않음 | 2주 |
| 5 | **음성 MVP 구축** | 오픈소스+상용 API 앙상블, 메타데이터·재인코딩 흔적·SynthID 확인, 3단 판정 PDF 리포트, 해시·모델 버전 기록 (8.3절 A) | 8~10주 |
| 6 | **자체 평가셋으로 오류율 측정·공개** | 최신 한국어 TTS로 동의 기반 합성 데이터를 만들어 오탐·미탐률 공개. 이것이 포지셔닝 B(공개 벤치마크) v0.1이 됨 | MVP와 병행 |
| 7 | **무료 파일럿 3~5곳** | 실제 사건 파일로 리포트 제공, "판정 불가" 비율과 고객 만족도 기록. 유료 전환 1곳 이상이 다음 단계 조건 | 3개월 차 |
| 8 | **자금·제도 경로 확보** | TIPS·정부 R&D 컨소시엄(IITP 2027년 과제, 경찰 과제 후속) 참여 탐색, 2028-04 총선 전 선관위 입찰 동향 추적 [디데일리](https://www.ddaily.co.kr/page/view/2026051314145159743) [다음](https://v.daum.net/v/6VGDUSx2ab) | 상시 |

**중단 신호(미리 정해 두라):** 인터뷰에서 유료 의향 고객이 3곳 미만이거나, 자체 평가셋 오탐률이 고객이 받아들일 수준으로 내려가지 않거나, FTO에서 핵심 기법이 막히면 접는다. 사용자가 처음 정한 "레드오션이면 포기" 원칙을 이 단계에서도 그대로 적용하는 것이다.


## 출처

본문에 인용한 출처 268개 (첫 인용 순).

1. [Reality Defender](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html)
2. [Pindrop](https://www.biometricupdate.com/202504/pindrop-surpasses-100m-in-annual-recurring-revenue-kicks-off-bu-podcast)
3. [Deezer](https://dataconomy.com/2026/01/29/music-streaming-giant-deezer-opens-ai-detection-tool-to-external-platforms/)
4. [GPTZero](https://www.businesswire.com/news/home/20260623083788/en/Superhuman-to-Acquire-GPTZero-AI-Authenticity-Platform)
5. [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/)
6. [Bitdefender](https://www.bitdefender.com/en-us/news/bitdefender-launches-realcheck-a-powerful-deepfake-detection-solution)
7. [CDT](https://cdt.org/insights/new-research-educators-still-struggling-with-generative-ai-detection-discipline-and-distrust-despite-increased-school-guidance/)
8. [AppBrain](https://www.appbrain.com/dev/Zyur/)
9. [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857)
10. [arXiv 2602.07814](https://arxiv.org/html/2602.07814)
11. [TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/)
12. [JUVE Patent](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/)
13. [Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents)
14. [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/)
15. [다음](https://v.daum.net/v/6VGDUSx2ab)
16. [바이라인](https://byline.network/2026/02/12-535/)
17. [Amped](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165)
18. [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364)
19. [GenImage](https://genimage-dataset.github.io)
20. [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877)
21. [arXiv 2402.03214](https://arxiv.org/pdf/2402.03214)
22. [BusinessWire](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats)
23. [Magnet](https://www.magnetforensics.com/blog/authenticity-on-trial-how-magnet-verify-helps-prosecutors-admit-digital-media-and-defeat-deepfake-defenses/)
24. [RD API](https://realitydefender.com/api)
25. [OpenAI](https://help.openai.com/en/articles/8912793-provenance-signals-content-credentials-synthid-in-openai-generated-content)
26. [arXiv 2604.24890](https://arxiv.org/pdf/2604.24890)
27. [DataInnovation](https://datainnovation.org/2025/08/5-qs-with-anatoly-kvitnitsky-ceo-of-ai-or-not/)
28. [Sightengine 가격](https://sightengine.com/pricing)
29. [GetReal](https://www.getrealsecurity.com/resources/getreal-security-raises-17-5m-series-a-led-by-forgepoint-capital-to-address-rapidly-growing-threats-associated-with-generative-ai-and-malicious-digital-media)
30. [뉴스핌](https://www.newspim.com/news/view/20260813000619)
31. [TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/)
32. [AppGoblin](https://appgoblin.info/apps/io.zyur.forgespy)
33. [c2paviewer](https://c2paviewer.com/articles/ai-tools-c2pa-support)
34. [ForensicFocus](https://www.forensicfocus.com/news/advanced-detection-tools-from-amped-software-aim-to-combat-ai-generated-csam-and-protect-children/)
35. [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/)
36. [arXiv 2608.10166](https://arxiv.org/pdf/2608.10166)
37. [SiliconANGLE](https://siliconangle.com/2021/04/21/enterprise-ai-solutions-startup-hive-raises-85m-2b-valuation/)
38. [HF 2606.19259](https://huggingface.co/papers/2606.19259.md)
39. [UPC 명령](https://www.unifiedpatentcourt.org/sites/default/files/files/api_order/922-2026%20Adobe%20ea%20Final%20Order%20en-GB.pdf)
40. [SecurityWeek](https://www.securityweek.com/getreal-security-raises-17-5-million-to-tackle-gen-ai-threats/)
41. [BusinessWire](https://www.businesswire.com/news/home/20251119488893/en)
42. [Chrome 웹스토어](https://chromewebstore.google.com/detail/hive-ai-detector/cmeikcgfecnhojcbfapbmpbjgllklcbi?hl=fil)
43. [McAfee](https://www.mcafee.com/en-us/newsroom/press-releases/2025/mcafees-scam-detector-added-to-core-plans-protecting-people-against-text-email-and-video-scams.html)
44. [Norton](https://support.norton.com/sp/en/us/home/current/solutions/v20250722122612120)
45. [Tubefilter](https://www.tubefilter.com/2026/05/18/youtube-generative-ai-deepfake-likeness-detection-rollout/)
46. [Android Central](https://www.androidcentral.com/apps-software/ai/gemini-can-now-tell-you-whether-a-video-was-generated-with-google-ai)
47. [Zoom](https://www.zoom.com/en/blog/zoomtopia2026-ai-governance-zoom-workplace/)
48. [BleepingComputer](https://bleepingcomputer.com/news/security/microsoft-teams-to-add-third-party-deepfake-detection-impersonation-protection)
49. [세계일보](https://www.segye.com/newsView/20260310517457)
50. [유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366)
51. [Gartner](https://www.gartner.com/en/documents/8056333)
52. [Google Play](https://play.google.com/store/apps/details?id=com.avk.imagehunter2&hl=en_US)
53. [Gigazine](https://gigazine.net/gsc_news/en/20260302-ai-detection-fake)
54. [DF26](https://arxiv.org/pdf/2609.07369)
55. [TechBytes](https://techbytes.app/posts/allure-security-17m-series-b-deepfake-fraud-prevention/)
56. [DF26](https://arxiv.org/html/2609.07369v1)
57. [Calcalist](https://www.calcalistech.com/ctechnews/article/bkeyex0sgl)
58. [ChatPaper](https://chatpaper.com/chatpaper/paper/357903)
59. [Mergermarket](https://ionanalytics.com/insights/mergermarket/pindrop-could-step-up-acquisitions-in-agentic-security-as-its-deepfake-detection-takes-off-ceo/)
60. [Pindrop](https://www.pindrop.com/article/pindrop-pulse-for-audio-deepfake-detection/)
61. [Resemble](https://www.resemble.ai/resources/audio-deepfake-detection-benchmark-results-how-8-systems-performed-in-2026)
62. [TechCrunch](https://techcrunch.com/2026/09/28/modulate-raises-25m-for-its-voice-models-and-analysis-suite/)
63. [SSN](https://www.securitysystemsnews.com/article/reality-defender-launches-public-api-and-free-tier)
64. [Google](https://blog.google/technology/ai/google-synthid-ai-content-detector/)
65. [ElevenLabs](https://elevenlabs.io/docs/eleven-creative/audio-tools/audio-detector)
66. [Hiya](https://www.hiya.com/press-releases/hiya-acquires-deepfake-voice-detection-leader-loccus-ai)
67. [eSecurityPlanet](https://www.esecurityplanet.com/cybersecurity/best-ai-deepfake-detection-tools/)
68. [바이라인](https://byline.network/2026/04/27-613/)
69. [디데일리](https://www.ddaily.co.kr/page/view/2025072908585835162)
70. [머니투데이](https://www.mt.co.kr/tech/2025/07/23/2025072315221813011)
71. [바이라인](https://byline.network/2026/09/11-703/)
72. [BiometricUpdate](https://www.biometricupdate.com/202603/zoom-expands-pindrop-deepfake-detection-to-customer-service)
73. [Hiya](https://blog.hiya.com/ai-is-making-voice-fraud-worse-both-in-volume-and-in-targeting)
74. [arXiv 2509.02859](https://arxiv.org/pdf/2509.02859)
75. [Engadget](https://www.engadget.com/google-is-banning-third-party-call-recording-apps-from-the-play-store-093201443.html)
76. [서울신문](https://m.seoul.co.kr/news/2024/04/01/20240401500181)
77. [한경](https://www.hankyung.com/article/2024110369981)
78. [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection)
79. [Pindrop](https://pindrop.com/products/liveness-detection)
80. [Winbuzzer](https://winbuzzer.com/2026/06/12/deezer-opens-free-ai-playlist-scanner-to-rival-services-xcxwbn/)
81. [AI Musicpreneur](https://www.aimusicpreneur.com/ai-tools-news/google-synthid-detector-public-launch-ai-music-october-2026/)
82. [Cyanite](https://cyanite.ai/blog/best-ai-music-detection-tools-2026/)
83. [MBW](https://musicbusinessworldwide.com/believe-has-developed-its-own-ai-made-music-detector-with-98-accuracy-what-might-this-mean-for-the-future)
84. [위키트리](https://www.wikitree.co.kr/articles/1137778)
85. [아시아경제](https://view.asiae.co.kr/article/2026083116360854659)
86. [PPC Land](https://ppc.land/spotify-drops-ai-persona-artists-from-recommendations-in-mid-september/)
87. [TechCrunch](https://techcrunch.com/2026/07/21/music-streamer-deezer-says-more-than-50-of-daily-uploads-are-ai-generated/)
88. [arXiv 2405.04181](https://arxiv.org/abs/2405.04181)
89. [Deezer](https://newsroom-deezer.com/2025/11/deezer-ipsos-survey-ai-music/)
90. [주간경향](https://weekly.khan.co.kr/article/202610130600011)
91. [iMusician](https://imusician.pro/en/resources/blog/deezer-demonetizes-85-of-ia-music-commercializes-ia-detection-technology)
92. [Deezer](https://newsroom-deezer.com/2025/01/deezer-deploys-cutting-edge-ai-detection-tool-for-music-streaming/)
93. [Wired](https://www.wired.com/story/student-papers-generative-ai-turnitin/)
94. [Turnitin FAQ](https://guides.turnitin.com/hc/en-us/articles/28477544839821-Turnitin-s-AI-writing-detection-capabilities)
95. [Startup Fortune](https://startupfortune.com/superhuman-bets-on-trust-as-it-buys-ai-detection-startup-gptzero-for-its-19-million-users-and-30m-arr/)
96. [BetaKit](https://betakit.com/grammarly-rebrands-to-superhuman-as-it-expands-from-catching-typos-to-ai-productivity/)
97. [NBER](https://www.nber.org/system/files/working_papers/w34223/w34223.pdf)
98. [BleepingComputer](https://www.bleepingcomputer.com/news/artificial-intelligence/openai-is-adding-invisible-watermarks-to-chatgpt-and-codex-text-in-the-eu/)
99. [Epoch AI](https://epoch.ai/data-insights/ai-detectors-false-negatives)
100. [Ars Technica](https://arstechnica.com/information-technology/2023/07/why-ai-detectors-think-the-us-constitution-was-written-by-ai/)
101. [아이티데일리](https://www.itdaily.kr/news/articleView.html?idxno=223370)
102. [지티티코리아](https://www.gttkorea.com/news/articleView.html?idxno=22638)
103. [AI킬러](https://aikiller.app/)
104. [OpenAI](https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/)
105. [Liang 외](https://arxiv.org/html/2304.02819v3)
106. [Plagiarism Today](https://www.plagiarismtoday.com/2026/02/11/adelphi-student-wins-ai-plagiarism-lawsuit/)
107. [Waterloo](https://uwaterloo.ca/educational-technology-hub/news/discontinuing-use-ai-detection-functionality-turnitin)
108. [ACL Anthology](https://aclanthology.org/2025.acl-long.1030)
109. [TechCrunch](https://techcrunch.com/2026/06/23/superhuman-acquires-ai-detection-startup-gptzero/)
110. [머니투데이](https://www.mt.co.kr/amp/future/2026/05/26/2026052609184984243)
111. [US11853708B1](https://patents.google.com/patent/US11853708B1/en)
112. [Gizmodo](https://gizmodo.com/bitdefender-built-an-app-that-analyzes-videos-for-deepfakes-so-you-dont-have-to-guess-2000780027)
113. [SecurityBrief](https://securitybrief.co.uk/story/norton-adds-ai-powered-deepfake-detection-to-genie-assistant)
114. [NPR](https://www.npr.org/2024/04/05/1241446778/deepfake-audio-detection)
115. [BusinessWire](https://www.businesswire.com/news/home/20260729222515/en/Pangram-Launches-New-Worlds-Best-AI-Detector-Expands-to-Images-Backed-by-$9M-From-Menlo-Ventures)
116. [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/)
117. [인공지능신문](https://www.aitimes.kr/news/articleView.html?idxno=34963)
118. [이투데이](https://www.etoday.co.kr/news/view/2439014)
119. [이데일리](https://edaily.co.kr/News/Read?mediaCodeNo=257&newsId=02725686628988568)
120. [Copyleaks](https://copyleaks.com/blog/ai-detector-apps-arent-what-they-claim)
121. [jakeinsight](https://jakeinsight.com/ko/tech-economy/2026-09-03-%EB%94%A5%ED%8E%98%EC%9D%B4%ED%81%AC-%ED%83%90%EC%A7%80%EA%B8%B0-%EC%95%B1-%EC%A7%84%EC%A7%9C-%EB%AF%BF%EC%96%B4%EB%8F%84-%EB%90%98%EB%82%98/)
122. [TrueMedia](https://www.truemedia.org/post/shutting-down-truemedia)
123. [Morgan Lewis](https://www.morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative)
124. [SocialMediaToday](https://www.socialmediatoday.com/news/youtube-expands-likeness-detection-to-all-users-over-18/820440/)
125. [C2PA FAQ](https://www.c2pa.org/faq)
126. [Google I/O](https://blog.google/innovation-and-ai/technology/ai/io-2026-keynote-moment-videos/)
127. [Lead Stories](https://leadstories.com/analysis/2026/07/google-gemini-synthid-detector-confuses-results-within-same-chat.html)
128. [InfoQ](https://infoq.com/news/2026/05/google-synthid-content-detection)
129. [MBW](https://www.musicbusinessworldwide.com/youtube-will-now-automatically-detect-and-label-ai-videos-even-when-creators-dont-disclose-it/)
130. [OpenAI 도움말](https://help.openai.com/en/articles/8912793-c2pa-in-chatgpt-images)
131. [The Star](https://www.thestar.com.my/tech/tech-news/2026/07/10/meta-ai-image-detector-fails-to-identify-some-of-its-own-cropped-ai-images-reuters-analysis-finds)
132. [TechCrunch](https://techcrunch.com/2025/11/18/tiktok-now-lets-you-choose-how-much-ai-generated-content-you-want-to-see/)
133. [ElevenLabs](https://elevenlabs.io/blog/synthid)
134. [Adobe](https://helpx.adobe.com/ae_en/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html)
135. [Nieman Lab](https://www.niemanlab.org/2026/09/apple-launches-a-new-way-to-prove-a-photo-was-shot-with-an-iphone-not-generated-by-ai/)
136. [Mixed](https://mixed-news.com/en/google-synthid-detector-worldwide-apple-ai-content-comes-soon/)
137. [InfoQ](https://infoq.com/news/2026/10/synthid-watermarking-detector)
138. [arXiv 2602.18681](https://arxiv.org/abs/2602.18681)
139. [AIID](https://incidentdatabase.ai/reports/6301)
140. [PetaPixel](https://petapixel.com/2025/02/13/samsungs-image-authenticity-approach-is-backward-and-its-ais-fault)
141. [AI Weekly](https://aiweekly.co/alerts/google-synthid-watermarks-hold-up-in-tests-labeling-still-slips)
142. [Gizmodo](https://gizmodo.com/metas-ai-detector-cant-detect-images-it-generated-itself-report-finds-2000784335)
143. [arXiv 2607.16010](https://arxiv.org/abs/2607.16010)
144. [DCW](https://www.digitalcameraworld.com/photography/photojournalism/nikon-revokes-all-c2pa-image-authenticity-certificates-after-major-vulnerability-exposed)
145. [arXiv 2512.11815](https://arxiv.org/abs/2512.11815v2)
146. [다음](https://v.daum.net/v/20260121120209717)
147. [The Decoder](https://the-decoder.com/microsofts-research-argues-ai-media-authentication-doesnt-work-reliably-yet-new-laws-assume-it-does/)
148. [뉴시스](https://www.newsis.com/view/NISX20260121_0003485509)
149. [ZDNet](https://zdnet.co.kr/view?no=20261020095628)
150. [트위그](https://www.twig24.com/news/2026/02/11/20260211500394)
151. [William Fry](https://www.williamfry.com/knowledge/eu-ai-act-omnibus-deal-reached-postponed-deadlines-watermarking-compromise-and-the-nudificiation-prohibition/)
152. [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/technology-quotient/eu-ai-act-unpacked-33-the-final-code-of-practice-on-transparency-of-ai-generate-102n4yx)
153. [Simmons](https://www.simmons-simmons.com/en/publications/cmoveo6ke00icuxskpgueb0od/ai-omnibus-update)
154. [FTC](https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-sends-warning-letters-companies-about-compliance-take-it-down-act)
155. [MoFo](https://www.mofo.com/resources/insights/261001-california-revamps-ai-transparency-requirements)
156. [Latham](https://www.lw.com/en/insights/newest-slate-of-ai-laws-keeps-california-at-the-forefront-of-us-regulation)
157. [TechNode](https://technode.com/2026/02/13/china-cyberspace-regulators-crack-down-on-unlabeled-ai-generated-content-penalize-over-13000-accounts/)
158. [Euronews](https://www.euronews.com/2026/10/08/denmark-introduces-a-bill-protecting-peoples-faces-and-voices-from-deepfakes)
159. [Ropes & Gray](https://www.ropesgray.com/en/insights/alerts/2025/12/trump-attempts-to-preempt-state-ai-regulation-through-executive-order)
160. [Morgan Lewis](https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative)
161. [Sheppard](https://www.sheppard.com/insights/blogs/california-enacts-ai-spokespeople-chatbots-and-content-disclosures-laws)
162. [arXiv 2605.09203](https://arxiv.org/pdf/2605.09203)
163. [OpenAI](https://openai.com/index/advancing-content-provenance)
164. [HF Papers](https://huggingface.co/papers/2503.02857)
165. [EmergentMind](https://www.emergentmind.com/topics/deepfake-eval-2024)
166. [DailyBench](https://arxiv.org/pdf/2607.24016)
167. [Müller 2022](https://arxiv.org/pdf/2203.16263)
168. [NIST](https://ai-challenges.nist.gov/t2i)
169. [NewsGuard](https://www.newsguardtech.com/?p=33448)
170. [The Star(NYT)](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work)
171. [CJR](https://www.cjr.org/tow_center/why-ai-models-are-bad-at-verifying-photos.php)
172. [PetaPixel](https://petapixel.com/2023/08/02/deepfake-detection-software-analyzes-a-persons-blood-flow)
173. [SiliconANGLE](https://siliconangle.com/2025/12/08/resemble-ai-hauls-13m-different-approach-deepfake-detection/)
174. [Reuters Institute](https://reutersinstitute.politics.ox.ac.uk/news/spotting-deepfakes-year-elections-how-ai-detection-tools-work-and-where-they-fail)
175. [TIGA](https://arxiv.org/pdf/2604.09706v1)
176. [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive)
177. [PhotoWorkout](https://www.photoworkout.com/?p=222434)
178. [한국경제](https://www.hankyung.com/article/2025121553117)
179. [뉴데일리](https://www.newdaily.co.kr/site/data/html/2025/12/15/2025121500350.html)
180. [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence)
181. [uscourts.gov](https://www.uscourts.gov/sites/default/files/document/advisory_committee_on_evidence_rules_may_2026.pdf)
182. [Volokh](https://reason.com/volokh/2025/09/25/court-throws-out-case-after-finding-plaintiffs-submitted-deepfake-videos-and-altered-images/)
183. [Amped 40960](https://blog.ampedsoftware.com/2026/06/25/authenticate-update-40960)
184. [Magnet](https://www.magnetforensics.com/blog/the-deepfake-detector-paradigm-shift-the-case-for-media-authentication-in-court/)
185. [Forensic Focus](https://www.forensicfocus.com/?p=507588)
186. [뉴스1](https://www.news1.kr/amp/local/moi/6096576)
187. [디지털데일리](https://www.ddaily.co.kr/page/view/2025020211334778803)
188. [바이라인네트워크](https://byline.network/2025/06/5-299/)
189. [보안뉴스](https://m.boannews.com/html/detail.html?idx=134010)
190. [TrueMedia 오픈소스](https://www.truemedia.org/post/open-source-release)
191. [뉴데일리](https://www.newdaily.co.kr/site/data/html/2026/08/13/2026081300088.html)
192. [경향](https://www.khan.co.kr/article/202504111006011)
193. [한국경제](https://www.hankyung.com/article/202603023306i)
194. [세계일보](https://www.segye.com/newsView/20250107509236)
195. [세계일보](https://www.segye.com/newsView/20240930510518)
196. [경향](https://www.khan.co.kr/article/202605281700001/)
197. [파이낸셜뉴스](https://www.fnnews.com/news/202605281717397963)
198. [아이뉴스24](https://www.inews24.com/view/2008688)
199. [파이낸셜뉴스](https://www.fnnews.com/news/202512101835084302)
200. [한국경제](https://www.hankyung.com/article/2026061601621)
201. [뉴시스](https://mobile.newsis.com/view/NISX20260604_0003655990)
202. [데일리안](https://www.dailian.co.kr/news/view/1408429/)
203. [korea.kr](https://www.korea.kr/news/policyNewsView.do?newsId=148973649)
204. [세계일보](https://www.segye.com/newsView/20250730515766)
205. [한경](https://www.hankyung.com/article/2026050722651)
206. [디데일리](https://www.ddaily.co.kr/page/view/2026051314145159743)
207. [서울시](https://mediahub.seoul.go.kr/archives/2014517)
208. [조달청](https://pps.go.kr/kor/content.do?key=00648)
209. [디데일리](https://www.ddaily.co.kr/page/view/2025111410120875507)
210. [머니투데이](https://www.mt.co.kr/future/2026/08/11/2026081109014616088)
211. [ZDNet](https://zdnet.co.kr/view/?no=20260918125809)
212. [AI타임스](https://www.aitimes.com/news/articleView.html?idxno=207851)
213. [알체라](https://www.alchera.ai/resource/blog/ekyc-deepfake-detection-identity-verification)
214. [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194)
215. [머니투데이](https://www.mt.co.kr/article/2026012216142218479)
216. [ITWorld](https://www.itworld.co.kr/article/3554516/%EC%98%81%EC%83%81%EC%9D%80-%EB%AC%BC%EB%A1%A0-%EC%9D%B4%EB%AF%B8%EC%A7%80%C2%B7%EC%9D%8C%EC%84%B1%EA%B9%8C%EC%A7%80-%EB%94%A5%EB%B8%8C%EB%A0%88%EC%9D%B8ai-%EB%94%A5%ED%8E%98.html)
217. [The VC](https://thevc.kr/deepbrainai/fundings)
218. [바이라인](https://byline.network/2026/01/13-583/)
219. [코리안센터](https://www.koreancenter.or.kr/news/articleView.html?idxno=1436290)
220. [한경](https://www.hankyung.com/article/202506260996i)
221. [코리안센터](https://www.koreancenter.or.kr/news/articleView.html?idxno=1434357)
222. [ITWorld](https://www.itworld.co.kr/article/3575761/%EB%94%A5%EB%B8%8C%EB%A0%88%EC%9D%B8ai-saas%ED%98%95-%EB%94%A5%ED%8E%98%EC%9D%B4%ED%81%AC-%ED%83%90%EC%A7%80-%EC%86%94%EB%A3%A8%EC%85%98-%EC%B6%9C%EC%8B%9C%EC%9D%8C%EC%84%B1-%ED%95%A9.html)
223. [K포렌식](https://digitalforensics.co.kr/)
224. [비석세스](https://besuccess.com/?p=185339)
225. [이화여대](https://ewha.libguides.com/GenAI/AIDetection)
226. [디지털투데이](https://www.digitaltoday.co.kr/en/view/91565/stealcut-deepfake-blocking-ai-security-startup-raises-seed-funding-from-mashup-ventures)
227. [머니투데이](https://www.mt.co.kr/tech/2025/12/31/2025123009504430416)
228. [특허뉴스](http://e-patentnews.com/14873)
229. [KISTI ScienceON](https://scienceon.kisti.re.kr/aiq/issue/selectIssueReportView.do?searchIssueRptNo=171&searchDataSectionId=tab_keyword)
230. [GT Law](https://www.gtlaw.com/en/insights/2025/4/federal-circuit-machine-learning-patents-ineligible-in-recentive-analytics-inc-v-fox-corp)
231. [Nixon Peabody](https://nixonpeabody.com/insights/alerts/2025/06/24/federal-circuit-limits-patent-eligibility-of-machine-learning-in-recentive-analytics-v-fox)
232. [USPTO 12586419](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586419)
233. [Justia](https://patents.justia.com/patent/12142083)
234. [USPTO 공보](https://patentsgazette.uspto.gov/week44/OG/html/1540-1/US12462813-20251104.html)
235. [USPTO 공보](https://patentsgazette.uspto.gov/week46/OG/html/1540-3/US12475695-20251118.html)
236. [Google Patents](https://patents.google.com/patent/US11687778)
237. [USPTO PDF](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586395)
238. [Justia](https://patents.justia.com/assignee/originality-ai-inc)
239. [TUM ToS](https://kaldir.vc.in.tum.de/faceforensics_tos.pdf)
240. [GitHub](https://github.com/sclbd/deepfakebench)
241. [ASVspoof 2019 논문](https://arxiv.org/pdf/1911.01601)
242. [AI Weekly](https://aiweekly.co/alerts/stanfords-gpic-ships-100m-commercially-usable-training-images)
243. [GitHub](https://github.com/truemediaorg/GenConViT)
244. [Google](https://ai.google.dev/responsible/docs/safeguards/synthid?hl=en)
245. [Meticulous](https://www.meticulousresearch.com/product/deepfake-detection-market-6944)
246. [SNS Insider](https://www.snsinsider.com/reports/deepfake-detection-market-11090)
247. [Astute](https://www.astuteanalytica.com/industry-report/deepfake-detection-market)
248. [Deloitte](https://www.deloitte.com/us/en/insights/industry/financial-services/deepfake-banking-fraud-risk-on-the-rise.html)
249. [HelpNetSecurity](https://helpnetsecurity.com/2026/09/29/pindrop-enterprise-deepfake-attacks-report)
250. [CyberScoop](https://cyberscoop.com/?p=87093)
251. [HelpNetSecurity](https://www.helpnetsecurity.com/2024/07/18/pindrop-financing-100-million/)
252. [DCVC](https://dcvc.com/press-releases/reality-defender-expands-series-a-to-33-million-to-enhance-ai-detection-capabilities)
253. [SecurityWeek](https://www.securityweek.com/doppel-raises-70-million-at-600-million-valuation/)
254. [Tech.eu](https://tech.eu/2026/03/12/neuramancer-lands-eur17m-pre-seed-to-scale-deepfake-detection-tools)
255. [AI Weekly](https://aiweekly.co/alerts/superhuman-acquires-gptzero-to-add-ai-authenticity-layer)
256. [BiometricUpdate](https://www.biometricupdate.com/202607/sensity-ai-gets-eic-funding-for-forensics-focused-deepfake-detection-models)
257. [Calcalist](https://calcalistech.com/ctechnews/article/bkeyex0sgl)
258. [Dealroom](https://dealroom.co/news/142736-deel-acquires-clarity-to-strengthen-identity-verification-surpasses-1-5b/)
259. [BiometricUpdate](https://www.biometricupdate.com/202609/kpmg-investment-in-reality-defender-backs-hiring-spree-to-fight-deepfakes)
260. [Sacra](https://sacra.com/c/turnitin/)
261. [CryptoBriefing](https://cryptobriefing.com/superhuman-acquires-gptzero-ai-detector/)
262. [SecurityWeek](https://www.securityweek.com/imper-ai-emerges-from-stealth-mode-with-28-million-in-funding/)
263. [Allwork](https://allwork.space/2025/04/ai-deepfake-scammers-infiltrating-the-hiring-processes-at-alarming-rates-gartner-reports/)
264. [Reinsurance News](https://www.reinsurancene.ws/coalition-enhances-cyber-product-with-addition-of-deepfake-response-endorsement)
265. [SecurityBrief](https://securitybrief.co.uk/story/norton-rolls-out-ai-deepfake-scam-protection-for-intel-pcs)
266. [Intercom 가격](https://intercom.help/reality-defender/en/articles/12831411-managing-your-plan-billing)
267. [Engadget](https://www.engadget.com/ai/a-new-chrome-extension-can-reliably-detect-ai-generated-voices-130059842.html)
268. [Simplify](https://simplify.jobs/c/Sensity)
