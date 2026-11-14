# AI 생성 영상·딥페이크 탐지: 검증 반영 요약본 (2026-11-14)

## 1. 영역 요약
- Gartner가 2026-06에 첫 딥페이크 탐지 스타트업 쿼드런트를 냈다. 이 보고서는 벤더의 규모와 시장 파괴 잠재력을 평가했으며 제품 정확도는 평가하지 않았다 ([RD 발표](https://www.realitydefender.com/insights/reality-defender-gartner-market-shaper), [SoftwareSeni](https://www.softwareseni.com/ai-deepfake-detection-market-reality-defender-getreal-96-vendor-accuracy-problem)).
- 소비자 쪽은 보안사의 번들 기능과 Bitdefender RealCheck 독립 앱(영어 전용)이 이미 차지하고 있다. 플랫폼들(Zoom, Teams)의 기능은 대부분 아직 출시 전이다 ([Bitdefender](https://www.bitdefender.com/en-us/news/bitdefender-launches-realcheck-a-powerful-deepfake-detection-solution), [Zoom](https://www.zoom.com/en/blog/zoomtopia2026-ai-governance-zoom-workplace/)).
- 독립 평가에서 최신 생성기 영상을 만나면 학술 탐지기는 우연 수준에서 약 70%까지 떨어진다. 상용 탐지기도 인간 분석가보다 못하다 ([DF26](https://arxiv.org/pdf/2609.07369), [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857)).
- 결론: 범용 탐지 앱·API는 레드오션이다. 특허 장벽은 낮지만 라이브니스·음성 분야는 예외다. 기술 문제가 풀리지 않았기 때문에 틈새는 남아 있다.

## 2. 주요 제품 표 (점수 1~5, 검증 반영)
| 제품 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| Reality Defender | Reality Defender(미국) | 플랫폼·API·회의 탐지 | 기업·정부 | 4 | 3 | 3 | 운영 중 | Gartner Market Shaper, KPMG 소수지분 투자(2026-09), 독립 벤치마크 없음 ([KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html)) |
| GetReal Security | GetReal(미국) | 포렌식·신원 플랫폼 | 기업·정부 | 4 | 3 | 3 | 운영 중 | 시리즈A 1,750만 달러, Market Shaper, 성능 비공개 ([SecurityWeek](https://www.securityweek.com/getreal-security-raises-17-5-million-to-tackle-gen-ai-threats/)) |
| Pindrop Pulse for Meetings | Pindrop(미국) | 콜센터·회의 실시간 탐지 | 기업 | 4 | 4 | 3 | GA(2025-11) | Zoom·Webex·Teams 지원, 음성이 주력 ([BusinessWire](https://www.businesswire.com/news/home/20251119488893/en)) |
| Hive AI Detector/API | Hive(미국) | API·Chrome 확장 | 플랫폼·국방·소비자 | 4 | 4 | 3 | 운영 중 | DIU 2년 계약 약 240만 달러, 우회 사례 보고됨 ([Hive PR](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats)) |
| Bitdefender RealCheck | Bitdefender(루마니아) | iOS/Android 독립 앱 | 소비자 | 4 | 2 | 2 | 출시(2026-06) | 구상 중인 앱과 가장 가까운 경쟁작, 영어 전용, 성능 비공개 ([Gizmodo](https://gizmodo.com/bitdefender-built-an-app-that-analyzes-videos-for-deepfakes-so-you-dont-have-to-guess-2000780027)) |
| Sensity AI | Sensity(네덜란드) | 웹·API·온프레미스 | 수사·KYC | 3 | 2 | 3 | 운영 중 | NYT 테스트 오디오 부문 최상위, 98%는 벤더 주장 ([The Star/NYT](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work)) |
| Resemble AI DETECT-3B | Resemble(미국) | API | 기업·정부 | 3 | 3 | 3 | 운영 중 | NYT 테스트 오디오 부문 최상위, 영상 근거 부족 ([The Star/NYT](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work)) |
| McAfee Deepfake/Scam Detector | McAfee(미국) | PC·모바일 번들 | 소비자 | 5 | 4 | 3 | 운영 중 | 코어 플랜 포함, 오디오 위주 분석 ([McAfee](https://www.mcafee.com/en-us/newsroom/press-releases/2025/mcafees-scam-detector-added-to-core-plans-protecting-people-against-text-email-and-video-scams.html)) |
| Norton Genie / Avast Deepfake Guard | Gen Digital(미국) | 구독 번들 | 소비자 | 5 | 3 | 2 | 운영 중 | YouTube 영어 영상 한정, Avast는 영어 오디오 한정 ([Norton 지원](https://support.norton.com/sp/en/us/home/current/solutions/v20250722122612120)) |
| YouTube 초상 감지 | Google(미국) | 플랫폼 내장 | 크리에이터 | 5 | 4 | 3 | 확대(2026-05) | 진위 판별이 아니라 본인 얼굴 매칭 방식 ([Tubefilter](https://www.tubefilter.com/2026/05/18/youtube-generative-ai-deepfake-likeness-detection-rollout/)) |
| Gemini SynthID 검증 | Google(미국) | 앱 업로드 검증 | 소비자 | 5 | 4 | 3 | 운영 중 | Google 워터마크가 있는 생성물만 판별 가능 ([Android Central](https://www.androidcentral.com/apps-software/ai/gemini-can-now-tell-you-whether-a-video-was-generated-with-google-ai)) |
| Zoom 딥페이크 위험 탐지 | Zoom(미국) | 유료 애드온 | 기업 | 5 | 1 | 2 | 미출시(2026-12~2027Q1 예상) | Zoom 스스로 "모든 것을 잡지 못한다"고 명시 ([Zoom](https://www.zoom.com/en/blog/zoomtopia2026-ai-governance-zoom-workplace/)) |
| Teams 서드파티 탐지 연동 | Microsoft(미국) | 인증 공급자 연동 통로 | 기업 | 5 | 1 | - | GA 11월 말~12월 중순 예상 | 탐지는 직접 하지 않고 연동만 제공, 데스크톱·웹 한정 ([BleepingComputer](https://bleepingcomputer.com/news/security/microsoft-teams-to-add-third-party-deepfake-detection-impersonation-protection), [M365 MC](https://mc.merill.net/message/RM573451)) |
| 경찰 탐지 SW / 국과수 모델 | 경찰청·국과수(한국) | 내부 도구 | 수사·선관위 | 4 | 3 | 3 | 운영 중 | 누적 1,636건 활용, 국과수 단일 모델 92%·앙상블 97% ([뉴스핌](https://www.newspim.com/news/view/20260813000619), [머니투데이](https://www.mt.co.kr/policy/2026/03/10/2026031015560960020)) |
| 딥브레인AI 탐지 솔루션 | 딥브레인AI(한국) | SaaS·API·AI 가드 | 공공·금융 | 3 | 3 | 3 | 운영 중 | 96%는 벤더가 의뢰한 KOLAS 시험 결과(재검증 못 함) ([유니콘팩토리](https://www.unicornfactory.co.kr/article/2025111111081151366)) |

참고: KYC 라이브니스(iProov, Jumio)는 별도 시장이다. Clarity는 2026-08 Deel에 인수됐다. TrueMedia는 2025-01 종료 후 Georgetown이 클로즈드 베타로 운영 중이다. Intel FakeCatcher와 MS Video Authenticator는 현황 미확인이다 ([Deel](https://www.deel.com/blog/deel-acquires-clarity/), [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/), [Intel](https://newsroom.intel.com/artificial-intelligence/intel-introduces-real-time-deepfake-detector)).

## 3. 4개 기준 판정
**메이저성: 높음(5).** 전문 스타트업(Reality Defender, GetReal, Pindrop, Hive), 대형 보안사(McAfee, Gen, Bitdefender), 플랫폼(YouTube, Gemini, Zoom, Teams)이 모두 들어와 있다 ([Gartner 문서](https://www.gartner.com/en/documents/8056333)). 다만 Zoom·Teams·삼성 기능은 아직 출시 전이므로 "플랫폼 내재화 완료"로 보면 과장이다 ([삼성 SG](https://news.samsung.com/sg/samsung-electronics-singapore-partners-with-reality-defender-to-advance-on-device-deepfake-detection-for-enterprises-in-singapore)).

**완성도·실사용: 중간(3).** B2B(콜센터, 채용, 모더레이션)는 실제로 쓰이고 있다. 독립형 소비자 도구는 채택이 미미하다. Hive 확장 사용자는 약 5만 명, 평점 4.6(417개)이다 ([Chrome 웹스토어](https://chromewebstore.google.com/detail/hive-ai-detector/cmeikcgfecnhojcbfapbmpbjgllklcbi?hl=fil)). 구글플레이 탐지 앱은 많아야 1만+ 다운로드다 ([Google Play](https://play.google.com/store/apps/details?id=com.avk.imagehunter2&hl=en_US)). NYT 테스트에서는 영상이 가장 취약한 영역이었고, 영상을 아예 지원하지 않는 서비스도 많았다 ([Gigazine](https://gigazine.net/gsc_news/en/20260302-ai-detection-fake)).

**신뢰도: 낮음(2).** 벤더는 95~99%를 주장하지만 독립 평가 결과는 다르다. Deepfake-Eval-2024에서 오픈소스 탐지기 AUC가 영상 50% 하락했고, 상용은 이보다 낫지만 인간 분석가에는 못 미쳤다 ([arXiv](https://arxiv.org/abs/2503.02857)). DF26에서는 학술 탐지기가 94.3에서 48.2로 떨어졌다 ([arXiv](https://arxiv.org/pdf/2609.07369)). 공공 기관 운영은 단일 탐지기만으로 확정하지 않는다. 선관위는 두 시스템이 모두 딥페이크로 판단할 때만 확정한다 ([세계일보](https://www.segye.com/newsView/20260310517457)).

**신규 진입 경쟁력: 범용은 낮음(2), 틈새는 중간(3).** 영상 단독 탐지 분야의 대형 투자는 2026년에 확인되지 않았다. 투자는 음성·사기·신원 쪽으로 쏠리고 있다 ([TechBytes](https://techbytes.app/posts/allure-security-17m-series-b-deepfake-fraud-prevention/)). 반면 재학습하면 AUROC 93.1 이상으로 회복된다는 결과가 있어, 데이터 운영 속도가 차별점이 될 수 있다 ([DF26](https://arxiv.org/html/2609.07369v1)).

## 4. 레드오션 판정: 부분적 (범용 = 예, 특화 = 아니오)
- **예(범용 앱·API):** 전문 기업, 보안사 번들, RealCheck(월 4.99달러), 플랫폼 기능이 이미 경쟁 중이다. 통합도 진행 중이다(Deel–Clarity, KPMG, Visa–BioCatch) ([Calcalist](https://www.calcalistech.com/ctechnews/article/bkeyex0sgl), [BiometricUpdate](https://www.biometricupdate.com/202608/visa-acquires-behavioral-biometrics-pioneer-biocatch-amid-fraud-prevention-build-up)).
- **아니오(특화):** 기술이 미해결이고(CCDF에서 10개 탐지기가 실패, [ChatPaper](https://chatpaper.com/chatpaper/paper/357903)), 한국어 지원이 비어 있으며(RealCheck 영어 전용), 법정 증거로 쓸 만한 수준은 아직 아무도 갖추지 못했다.
- **특허:** 영상 탐지 전반을 막는 단일 특허는 확인되지 않았다. 라이브니스는 FaceTec 특허 4건이 PTAB에서 유지됐고(Jumio IPR, 등록 특허 50건), 음성은 Pindrop 포트폴리오가 크다. 정식 FTO는 하지 않았다 ([BiometricUpdate](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents), [IDTechWire](https://idtechwire.com/facetec-reaches-50-issued-patents-with-uspto-grant-on-autonomous-authentication-nodes/)).

## 5. 빈틈·기회
- **한국어·국내 플랫폼 특화:** RealCheck, Norton, Avast는 영어 전용이다 ([Bitdefender FR](https://www.bitdefender.com/fr-fr/news/bitdefender-lance-sa-solution-realcheck-pour-detecter-les-deepfakes-et-les-contenus-rauduleux), [Norton 지원](https://support.norton.com/sp/en/us/home/current/solutions/v20250722122612120)).
- **포렌식 감정서형 리포트와 다중 모델 합의:** 국과수·선관위의 앙상블·이중 합의 방식이 공공 감정의 실제 운영 기준이다 ([머니투데이](https://www.mt.co.kr/policy/2026/03/10/2026031015560960020)).
- **디지털 성범죄 대응 연계:** 2026년 1~7월 419명 검거, 17명 구속 ([파이낸셜뉴스](https://www.fnnews.com/news/202608131007468569)). 미국 TAKE IT DOWN Act는 48시간 내 삭제와 건당 53,088달러 민사벌을 규정해 플랫폼용 탐지·중복 제거 수요를 만든다 ([FTC](https://search.ftc.gov/news-events/news/press-releases/2026/05/ftc-begins-enforcing-take-it-down-act)). EU는 2026-12-02부터 누디파이·CSAM 생성 AI를 금지한다 ([Simmons](https://www.simmons-simmons.com/en/publications/cmoveo6ke00icuxskpgueb0od/ai-omnibus-update)).
- **열화 영상(재공유, CCTV) 특화:** CCDF와 RA-Bench가 공통으로 지적한 약점이다 ([ChatPaper](https://chatpaper.com/chatpaper/paper/357903), [HF RA-Bench](https://huggingface.co/papers/2608.14391)).
- **Teams 인증 공급자, Zoom 마켓플레이스 유통:** 기회이지만 인증 요건이 문턱이다 ([Windows Latest](https://windowslatest.com/2026/10/25/microsoft-confirms-teams-will-let-third-party-tools-scan-your-meetings-for-deepfakes-from-november)).
- **지속 재학습 운영(MLOps)과 버티컬 시장(보험, 채용):** ([DF26 데이터셋](https://huggingface.co/datasets/DF26/DF26), [Attestiv](https://www.globenewswire.com/news-release/2025/02/27/3033801/0/en/Attestiv-Video-Deepfake-Detection-Adds-Context-Analysis-Using-AI-to-Further-Uncover-Deepfake-Threats.html)).

## 6. 위협·장벽
- **군비경쟁:** DF26 성능 붕괴처럼 새 생성기가 나올 때마다 재학습 비용이 든다. TrueMedia는 운영비 부담으로 종료했다 ([GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/)).
- **무료 번들과 플랫폼 내장:** McAfee, Norton, Gemini, YouTube가 무료 또는 구독 포함으로 제공한다 (위 표 출처).
- **신원 증명으로의 전환:** Zoom–World ID, Teams 사칭 보호가 실시간 회의 탐지 시장을 줄일 수 있다 ([TNW](https://thenextweb.com/news/zoom-world-id-deep-face-verify-human-meetings-deepfake)).
- **자금력 격차:** Pindrop은 누적 약 3.18억 달러, RD는 누적 약 4,000만~5,200만 달러를 조달했다 ([SecurityWeek](https://www.securityweek.com/pindrop-security-raises-100-million-to-expand-deepfake-detection-technology/amp/), [BiometricUpdate](https://www.biometricupdate.com/202609/kpmg-investment-in-reality-defender-backs-hiring-spree-to-fight-deepfakes)).
- **오탐 책임과 증거능력:** BBC 테스트에서 FakeCatcher가 실제 영상을 오탐했다. 미국 FRE 707은 제정이 지연되고 있다 ([BBC 테스트 보도](https://www.advanced-television.com/2023/07/24/bbc-tests-intel-deepfake-detector), [Bloomberg Law](https://news.bgov.com/bloomberg-law-analysis/analysis-proposed-fre-707-stalls-but-is-that-such-a-bad-thing)).
- **워터마크 제거, 공공 조달:** Sora 워터마크는 약 4분 만에 제거됐다 ([Decrypt](https://decrypt.co/345296/sora-2-fabricate-convincing-deepfakes-on-command-study-finds)). 경찰·국과수는 자체 도구를 쓰고, 국내에는 정부 과제 수행사(누리랩 등)도 있다 ([보안뉴스](https://m.boannews.com/html/detail.html?idx=137309)).

## 7. 핵심 사실 목록
- **독립 평가:** DF26은 실제 271개, 합성 2,420개 클립을 7개 생성기로 만들었다. 기존 94.3이던 AUROC가 48.2로 떨어졌고, 최고 모델은 69.7, 인간은 52.6%였다. 대상은 FF++로 학습한 학술 탐지기다 ([arXiv](https://arxiv.org/pdf/2609.07369), [Unite.AI](https://www.unite.ai/deepfake-detection-accuracy-falls-49-in-a-year-of-ai-video-progress/)).
- **독립 평가:** Deepfake-Eval-2024는 88개 사이트, 52개 언어의 실제 유포 콘텐츠로 만들었다. 오픈소스 AUC가 영상 50%, 음성 48%, 이미지 45% 하락했다 ([arXiv](https://arxiv.org/abs/2503.02857)).
- **독립 평가:** CCDF는 실제 460개와 생성 1,380개(범죄·사고 16개 범주)로 구성되며, 10개 탐지기가 안정적으로 구분하지 못했다 ([ChatPaper](https://chatpaper.com/chatpaper/paper/357903)).
- **독립 평가:** NYT가 12개 서비스를 1,000회 이상 스캔했다. 영상이 가장 취약했고, 오디오는 Sensity와 Resemble이 가장 나았다 ([The Star](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work)).
- **벤더 주장:** RD 95~99%(실험실 기준), Hive 98%+, Sensity 98%, McAfee 영상 96%, 딥브레인AI 96% ([RD](https://www.realitydefender.com/insights/executing-deepfake-detection-in-real-world-settings), [Axios](https://www.axios.com/2024/08/21/deepfake-detector-mcafee-ai-detection-tool)).
- **요금:** RealCheck Core 월 4.99달러(200회), Plus 월 12.99달러(600회), 7일 체험 ([Bitdefender](https://www.bitdefender.com/en-us/news/bitdefender-launches-realcheck-a-powerful-deepfake-detection-solution)). RD는 무료 50회(영상 불가), Developer 월 399달러에 1,000회 ([RD 헬프](https://intercom.help/reality-defender/en/articles/12831411-managing-your-plan-billing)).
- **M&A:** Clarity 인수가는 비공개이며 4,000만~5,000만 달러로 추정된다. 시드는 1,600만 달러였다 ([TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection)). Visa는 BioCatch를 24억 달러에 인수하기로 했다 ([TNW](https://thenextweb.com/news/visa-biocatch-2-4-billion-acquisition-fraud-ai-scams)).
- **규제:** EU 제50조 표시 의무는 2026-08-02부터 시행됐고, 기계판독 워터마크만 기존 시스템에 한해 2026-12-02까지 유예된다 ([Usercentrics](https://usercentrics.com/knowledge-hub/eu-ai-act-high-risk-delay-article-50-transparency-consent/)). 한국 AI기본법은 2026-01-22 시행됐지만 과태료는 1년 이상 계도기간 동안 유예된다 ([비즈워치](https://news.bizwatch.co.kr/article/mobile/2026/01/21/0018)).
- **수요:** Arup은 화상회의 딥페이크로 약 2,500만 달러를 잃었다 ([CFO Dive](https://www.cfodive.com/news/deepfake-scam-engineering-firm-arup-25-million-fraud-hong-kong-cfo/716501/)). 선관위 딥페이크 삭제 요청은 388건(2024)에서 10,510건(2025)으로 늘었다 ([뉴스1](https://www.news1.kr/local/moi/6096576)).
- **시장 규모:** 리서치사 추정치로 2026년 약 7억~10억 달러, 영상 점유율 39.2% ([Meticulous](https://www.meticulousresearch.com/product/deepfake-detection-market-6944)).

## 8. 검증에서 정정·삭제된 주요 사항
- **"상용 실환경 약 78%" → 미확인으로 강등:** Deepfake-Eval-2024 초록에 없는 수치로, RD 블로그의 2차 인용이다. 신뢰도 논거로 쓰지 말 것.
- **DF26 붕괴 수치:** 학술 탐지기(FF++ 학습) 기준이다. 상용 제품 전체로 일반화하면 과장이다.
- **RealCheck "14개국" → 미확인:** 보도된 시장은 미국·영국·호주·캐나다·독일·프랑스·이탈리아·스페인 등이고, 영어로만 제공된다.
- **Teams "11월 정식 출시" → 정정:** Targeted Release 11월 중하순, GA 11월 말~12월 중순 예상이다. 모바일은 미지원이다.
- **Zoom 출시 시점:** 2026-12~2027Q1 예상이며 확정되지 않았다. 삼성 MoU는 싱가포르 기업용이고 출시일 미정이다.
- **CCDF 1,840개 → 실제 영상을 포함한 전체 수:** AUC 0.515와 arXiv ID는 미확인이다.
- **Hive 확장:** 평점 4.7(411개) → 4.6(417개)로 정정. "이미지 중심" 서술은 삭제한다(영상·텍스트·오디오도 지원).
- **FaceTec:** PTAB 결정은 Jumio IPR에 대한 것이다. iProov는 별건 소송(반소 제기)이고, PTAB은 침해 여부를 판단하지 않는다.
- **국과수 92%:** 단일 모델 수치다. 앙상블은 최대 97%다. 경찰 "도입 시 80%" 수치는 2024년 기사 기준이며 재확인하지 못했다.
- **규제 추가·정정:** 한국 과태료는 계도기간 동안 유예된다. EU 누디파이 금지(2026-12-02)와 미국 TAKE IT DOWN Act 집행(2026-05-19)을 추가했다.
- **재검증하지 못한 항목(미확인):** RD 특허 건수, 딥브레인AI 96% KOLAS, Sensity EIC 지원, Resemble 1,300만 달러, Hive 시리즈E, Arup·북한 IT 인력 수치.
