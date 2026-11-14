# 탐지 기술의 실제 신뢰도와 포렌식 수준 요건: 검증 반영 요약본

기준일 2026-11-14. 원 조사(reliability.research.json)에 2차 적대적 검증(실제 웹 검색 15회, WebFetch 없음)을 반영했다. 1차 검증(reliability.verify.json)은 검색 없이 끝나 반영하지 않았다. 표기 규칙은 다음과 같다. "독립 평가"는 제3자 테스트, "벤더 주장"은 회사·정부의 자체 발표다. "미확인"은 이번 검증에서 원문을 확인하지 못한 항목, "미확인(사전 지식)"은 검색 근거 없이 사전 지식에만 기댄 내용이다.

## 1. 영역 요약

- 실제 유통 딥페이크로 만든 벤치마크에서 오픈소스 SOTA 탐지기의 AUC는 학술 벤치마크 대비 45~50% 떨어졌다. 상용 모델은 오픈소스보다 낫지만 인간 포렌식 분석가에는 못 미쳤다 [Deepfake-Eval-2024](https://arxiv.org/abs/2503.02857).
- 언론 독립 감사(NewsGuard, NYT)에서는 오탐과 미탐 사이의 트레이드오프가 뚜렷했다. 어떤 도구도 두 가지를 동시에 잘하지 못했다 [NewsGuard](https://www.newsguardtech.com/?p=33448).
- 포렌식 벤더(Amped, Magnet)와 국과수·선관위는 AI 분류기를 스크리닝 용도로만 쓴다. 최종 판단은 다중 기법과 전문가에게 맡긴다 [Amped 40165](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165).
- 미국 연방증거규칙 Rule 707은 2026년에 두 차례 보류됐다. 시행은 빨라야 2029-12로 분석된다. 증거능력 기준의 공백은 오래 갈 전망이다 [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence).
- 범용 점수형 탐지기 시장은 통합 단계(Gartner 카테고리 신설, Deel의 Clarity 인수, KPMG 투자)에 들어선 레드오션이다. 소규모 팀의 현실적 목표는 트리아지 보조 도구나 도메인 특화 모델이다.

## 2. 주요 제품 표 (중요도 순)

점수는 1~5이며 괄호 안은 원 조사 대비 조정 내역이다.

| 제품 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| Hive AI-Generated/Deepfake Detection | Hive(미국) | API·온프레미스 | 플랫폼·정부 | 4 | 4 | 3 (4→3) | 운영중 | DIU가 36개사 중 선정, 2년 240만 달러(프로토타입 계약)였다. 같은 보도에 우회 연구가 언급되고, NewsGuard에서 조작 이미지 탐지율은 73%였다 [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive) |
| Reality Defender | Reality Defender(미국) | API·실시간 음성 | 금융·콜센터·정부 | 4 | 3~4 (3→3~4) | 3 | 운영중 | Series A 3,300만 달러(2024-10), Gartner Market Shaper(2026-06), KPMG 소수 지분 투자(2026-09) [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html) |
| Amped Authenticate | Amped Software(이탈리아) | 데스크톱 포렌식 SW | 수사기관·감정인 | 4 | 3 | 3 | 운영중(2026-06 비디오 확산모델 탐지 추가) | AI 탐지는 '스크리닝용'이라고 명시하고 결과에 모델 버전을 기록한다 [Amped 40960](https://blog.ampedsoftware.com/2026/06/25/authenticate-update-40960) |
| Magnet Verify(구 Medex) + Axiom Magnet Copilot | Magnet Forensics(캐나다/미국) | 파일 구조 기반 인증 SW | 수사기관 | 4 | 3 | 3 | 운영중. AI 판별은 Axiom 8.0 얼리 액세스 | '탐지보다 인증'을 표방한다. 인수 시점(2024-08)은 미확인 [Forensic Focus](https://www.forensicfocus.com/interviews/jad-saliba-founder-chief-innovation-officer-magnet-forensics/) |
| 국과수·행안부 딥페이크 분석모델 | 국과수/행안부(한국) | 정부 내부 감정 시스템 | 경찰·선관위 | 4 | 3 | 3 | 운영중(2026-03 선관위 제공) | 정확도 76%→92%는 정부 자체 발표(벤더 주장)이고 독립 검증이 없다 [세계일보](https://www.segye.com/newsView/20260310517457) |
| AI or Not | Optic(미국) | 소비자 웹·API | 소비자·기업 | 2 | 3 | 3 | 운영중 | NewsGuard 오탐 6.7%, 조작 이미지 탐지 100%였다. 다만 리터치 사진도 87%를 AI로 판정했다. NYT 비교에서 상위 4개에 들었다 [NewsGuard](https://www.newsguardtech.com/?p=33448) |
| Resemble Detect | Resemble AI(미국) | 음성·이미지 API | 기업 | 3 | 2 | 3 | 운영중 | NYT에서 복잡한 AI 이미지를 맞힌 4개 중 하나이고, 오디오 7개 도구 중 최상위였다 [The Star(NYT)](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work) |
| Sensity AI | Sensity(네덜란드) | API·플랫폼 | KYC·정부 | 3 | 2 | 3 | 운영중 | NYT 오디오 테스트에서 Resemble과 함께 최상위였다. Deepfake-Eval의 벤더별 수치는 익명이다 [The Star(NYT)](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work) |
| GetReal Security | GetReal(미국, Hany Farid) | 포렌식 SaaS·API | 기업 보안·정부 | 3 (4→3) | 2 | 3 | 운영중 | Series A 1,750만 달러(2025-03, Forgepoint 주도, In-Q-Tel·Cisco·Capital One 참여). 공개 성능 데이터는 없다 [GetReal](https://www.getrealsecurity.com/resources/getreal-security-raises-17-5m-series-a-led-by-forgepoint-capital-to-address-rapidly-growing-threats-associated-with-generative-ai-and-malicious-digital-media) |
| Sightengine | Sightengine(프랑스) | API | 플랫폼 | 3 | 3 | 2 (3→2) | 운영중 | NewsGuard 오탐 0%였지만 조작 이미지는 33%만 탐지했다. 적대적 전이 공격에도 취약하다 [NewsGuard](https://www.newsguardtech.com/?p=33448) |
| Clarity(Deel 인수) | Clarity(이스라엘) → Deel | 신원·화상 딥페이크 탐지 | HR·신원확인 | 3 | 2 | 미확인 | 2026-08 인수 | 추정 인수가 4,000만~5,000만 달러, 누적 투자 1,600만 달러 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection) |
| 경찰청 판별 시스템 / 딥브레인AI | 숭실대 컨소시엄, DeepBrain AI(한국) | 수사기관용 SW | 경찰·수사기관 | 3 | 2 | 2 | 개발 중(2025-04~2027-12) | 3년 91억 원 국책과제다. 딥브레인AI의 520만 건 학습은 벤더 주장 [디지털데일리](https://www.ddaily.co.kr/page/view/2025020211334778803) |
| TrueMedia.org 탐지기 | TrueMedia → Georgetown(미국) | 웹 → 오픈소스(MIT) | 언론·팩트체커 | 3 | 2 (3→2) | 3 | 2025-01 종료, Georgetown 클로즈드 베타 | 높은 운영비로 종료했다 [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/), [TrueMedia](https://www.truemedia.org/how-it-works) |
| ZeroGPT Image Detector | ZeroGPT(미확인) | 소비자 웹 | 소비자 | 2 | 3 | 2 | 운영중 | NewsGuard 오탐 20%, 조작 이미지 탐지 93.3% [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/) |
| Intel FakeCatcher | Intel(미국) | rPPG 기반 서버 | 기업·미디어 | 2 (5→2) | 1 | 2 | 2023년 이후 활동 미확인 | 벤더 주장 96%. 독립 평가인 BBC 테스트에서 진짜 영상을 여러 번 오탐했다 [Advanced Television](https://www.advanced-television.com/2023/07/24/bbc-tests-intel-deepfake-detector) |

ScamAI는 NewsGuard 오탐률 40%(6/15)로 최악이었고 영향력이 작아 표에서 뺐다 [NewsGuard](https://www.newsguardtech.com/?p=33448). Cellebrite는 2026 가을 릴리스가 에이전틱 AI 'Genesis' 중심이었고, 전용 딥페이크 탐지 기능은 검색에서 확인되지 않았다(검색 1회 결과라 확정 아님) [Forensic Focus](https://www.forensicfocus.com/?p=507588).

## 3. 4개 기준 판정

**메이저성.** 이미 메이저가 있다. 플랫폼·정부용 API는 Hive와 Reality Defender, 수사기관용은 Amped와 Magnet이 축이다. Gartner가 2026-06 'Emerging Market Quadrant for Deepfake Detection'을 신설해 독립 카테고리로 인정했다 [BiometricUpdate](https://www.biometricupdate.com/202609/kpmg-investment-in-reality-defender-backs-hiring-spree-to-fight-deepfakes). 한국 공공 영역은 국과수 모델과 경찰청 국책과제가 선점했다. 소비자 영역(AI or Not, ZeroGPT)은 인지도는 있으나 지배적 1위가 없다.

**완성도·실사용.** B2B·정부 업체는 투자, 계약, M&A로 실사용 신호가 뚜렷하다. Reality Defender는 KPMG 투자를 받았고, Clarity는 Deel에 인수됐으며, Hive는 DIU 계약을 따냈다 [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html). 반대로 무료 공익형 TrueMedia는 운영비 때문에 종료하고 클로즈드 베타로만 남았다 [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/). 고객 수, MAU, 매출 같은 공개 수치는 거의 없다.

**신뢰도.** 실제 환경에서 단독으로 감정 근거가 될 수 있는 탐지기는 없다(독립 평가). Deepfake-Eval-2024에서 상용 모델도 인간 분석가에 미달했고 [arXiv](https://arxiv.org/abs/2503.02857), NewsGuard에서는 오탐 0%인 도구(Hive, Sightengine)가 조작 이미지의 27~73%만 잡았다 [NewsGuard](https://www.newsguardtech.com/?p=33448). 벤더 정확도 수치는 대부분 비공개이거나 자체 발표다(Intel 96%, 국과수 92%). 정부 독립 벤치마크(NIST GenAI 이미지 판별)의 결과 수치는 2026-11 현재도 공개되지 않았다 [NIST](https://ai-challenges.nist.gov/t2i).

**신규 진입 경쟁력.** 범용 점수형으로는 낮다. 시장이 통합 단계이고 대형 업체·컨설팅사가 기업 채널을 흡수하고 있다 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection). 경쟁력이 생길 수 있는 지점은 설명 가능한 감정서형 리포트, '판정 불가'를 포함한 보정 출력과 공개 오류율, 부분 조작 위치 표시, 출처증명 결합, 한국어·도메인 특화다. 수사 시장은 기술 공백이 있지만 조달 채널, 증거능력 기준 공백(2029년 이후), 국책과제 선점 때문에 진입 장벽이 높다.

## 4. 레드오션 판정: 부분적

- **예: 범용 'AI 생성 여부 점수' 탐지기.** 수십 개 서비스가 경쟁하고, Gartner 카테고리가 생겼으며, M&A(Deel-Clarity)와 빅4 투자(KPMG-Reality Defender)가 이어지는 통합 단계다 [TechFundingNews](https://techfundingnews.com/deel-buys-deepfake-detection-startup-clarity-in-15th-acquisition-as-it-hits-1-5b-in-arr/).
- **아니오: 기술 측면의 '수사 수준'.** 아무도 실제 환경에서 단독 감정 수준에 도달하지 못했다 [arXiv](https://arxiv.org/abs/2503.02857).
- **단, 블루오션도 아니다.** 수사기관 채널은 Amped·Magnet이 쥐고 있고, 국내는 국과수와 경찰청 91억 원 과제가 선점했다. 증거능력 기준도 최소 2029년까지 공백이다 [Proskauer](https://www.proskauer.com/blog/machine-generated-evidence-challenges-the-federal-rules-inside-the-contested-proposed-federal-rule-of-evidence-707).
- **특허.** 결정적 특허 장벽은 '확인하지 못함'이지 '없음'이 아니다(검증 예산 부족으로 미검증). rPPG(Intel) 등 개별 기법의 특허는 별도 FTO 조사가 필요하다(미확인(사전 지식)).

## 5. 빈틈·기회

- **감정서형 설명 리포트.** 판단 근거 신호(주파수, PRNU, 메타데이터·컨테이너, 조명·기하, 립싱크), 모델 버전, 해시, 증거 보관 연속성을 함께 남긴다. Amped가 모델 버전 컬럼을 추가한 것이 이 수요의 신호다 [Amped 40165](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165).
- **진짜/가짜/판정 불가 3단 출력과 공개 오류율.** 소비자 도구의 오탐은 최대 40%였다 [NewsGuard](https://www.newsguardtech.com/?p=33448). 선관위는 기존 프로그램과 국과수 모델이 모두 딥페이크로 판단할 때만 확정하는 AND 규칙을 쓴다. 교차검증용 보조 모델로 들어갈 여지가 있다 [뉴스1](https://www.news1.kr/amp/local/moi/6096576).
- **부분 조작 탐지와 위치 표시.** 오탐이 적은 도구도 조작 이미지를 27~73%만 잡았다 [NewsGuard](https://www.newsguardtech.com/?p=33448).
- **원본·출처 분석 중심의 음성 감정 보조.** 김수현 녹취 사건에서 국과수 '판정 불가'의 사유는 원본이 아니고 잡음이 많다는 것이었다. 원본 메타데이터, 편집 흔적, 버전 비교 기능에 대한 요구가 보인다 [뉴데일리](https://www.newdaily.co.kr/site/data/html/2025/12/15/2025121500350.html).
- **출처증명(C2PA, SynthID)과 수동 탐지의 하이브리드.** 남는 시장은 워터마크가 없는 오픈소스 생성물과 부분 편집이다(미확인(사전 지식)).
- **한국어·한국 플랫폼 특화.** 카카오톡 압축 경로, 한국어 보이스피싱 음성 등이다. 딥브레인AI도 한국인 데이터를 강점으로 내세운다(벤더 주장) [CIO](https://www.cio.com/article/3516859/).
- **소규모 팀 포지션과 출구.** 감정인·기자용 트리아지, 도메인 특화 모델(보험 사진, 음성 사기, 학교 딥페이크 1차 선별), 오픈소스(TrueMedia MIT 공개 모델)와 상용 API를 묶는 앙상블 레이어가 가능하다. M&A 기준점은 Clarity(누적 투자 1,600만 달러, 추정 인수가 4,000만~5,000만 달러)다 [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection), [TrueMedia 오픈소스](https://www.truemedia.org/post/open-source-release).

## 6. 위협·장벽

- **일반화 실패.** GenImage에서 90%를 넘던 탐지기가 최신 세트(DailyBench)에서 약 57%로 떨어진다 [DailyBench](https://arxiv.org/pdf/2607.24016). 음성은 ASVspoof 2019로 학습한 모델의 EER이 In-the-Wild에서 200~1000% 악화됐다 [Müller 2022](https://arxiv.org/pdf/2203.16263). 지속적인 재학습 비용이 구조적으로 든다. 이 두 항목은 2차 검증 대상이 아니었다.
- **적대적 우회.** 해상도를 낮추고 끝부분을 자르자 판정이 뒤집혔다 [Reuters Institute](https://reutersinstitute.politics.ox.ac.uk/news/spotting-deepfakes-year-elections-how-ai-detection-tools-work-and-where-they-fail). TIGA 공격은 0.25배 다운샘플링 뒤에도 78% 우회율을 유지했다 [TIGA](https://arxiv.org/pdf/2604.09706v1). Hive도 이미지 조작으로 우회할 수 있다는 연구가 보도됐다 [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive).
- **오탐의 법적·평판 리스크와 거짓말쟁이의 배당.** 진짜 참상 사진이 조작으로 판정됐다 [PhotoWorkout](https://www.photoworkout.com/?p=222434). 김수현 사건에서는 한쪽이 '판정 불가'를 '완승'으로 선전했다 [한국경제](https://www.hankyung.com/article/2025121553117).
- **증거능력 문턱.** Rule 707은 2026-05 자문위원회와 2026-06 Standing Committee에서 연달아 진척되지 않았다. 시행은 빨라야 2029-12-01로 분석된다. 그 전까지는 Daubert/702 수준의 오류율 공개와 검증이 필요하다 [Redgrave](https://www.redgravellp.com/publication/machine-generated-evidence--rules-advisory-committee-hits-pause-to-consider-significant-revisions-to-proposed-federal-rule-of-evidence-707-addressing-evidence-generated-by-artificial-intelligence), [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence). ISO/IEC 17025 인정, SWGDE·ENFSI 가이드라인 같은 감정기관 요건도 있다(미확인(사전 지식)).
- **기존 채널과 정부 내재화.** 국내는 국과수 모델(선관위 제공)과 경찰청 91억 원 사업이 있다. 이 사업은 개발 후 모든 수사기관이 공동 활용하는 시스템으로 구축할 계획이다 [바이라인네트워크](https://byline.network/2025/06/5-299/).
- **데이터 장벽.** 실전 딥페이크(성범죄물, 범죄 음성)는 법적으로 수집·보관이 어렵고 전문가 라벨링이 필요하다(원 조사 판단, 직접 출처 없음).
- **비즈니스 모델.** 무료 공익형은 운영비로 종료했다(TrueMedia). B2B·정부 조달은 영업 주기가 길다 [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/).

## 7. 핵심 사실 목록

1. **(독립 평가, 확인)** Deepfake-Eval-2024: 88개 사이트, 52개 언어, 비디오 45시간, 오디오 56.5시간, 이미지 1,975장. 오픈소스 SOTA의 AUC가 비디오 50%, 오디오 48%, 이미지 45% 하락했다(하락률은 오픈소스 기준). 상용 모델은 오픈소스보다 낫지만 포렌식 분석가에 미달했다 [arXiv](https://arxiv.org/abs/2503.02857), [HF Papers](https://huggingface.co/papers/2503.02857).
2. **(독립 평가, 미확인)** 같은 벤치마크에서 '상용 22개 중 정확도 90% 이상 없음', '이미지 최고 상용 AUC 0.90 대 오픈소스 0.56', 'CVPRW 2026 게재'는 원문 대조를 못 했다. 2차 집계에는 최고 상용 비디오 탐지기 정확도가 약 78%로 나와 있다 [EmergentMind](https://www.emergentmind.com/topics/deepfake-eval-2024).
3. **(독립 평가, 확인)** NewsGuard(2026-05-08, 진짜 15장, 조작 15장). 진짜 사진 오탐률은 ScamAI 40%, ZeroGPT 20%, AI or Not 6.7%, Hive·Sightengine 0%. 조작 이미지 탐지율은 AI or Not 100%, ZeroGPT 93.3%, ScamAI 80%, Hive 73%, Sightengine 33%. Hive는 가벼운 리터치를 27%만 탐지했다. 표본이 작아 일반화하기는 어렵다 [NewsGuard](https://www.newsguardtech.com/?p=33448), [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/).
4. **(독립 평가, 확인)** NYT(2026-02-25) 12개 서비스 비교에서 복잡한 AI 이미지를 맞힌 서비스는 AI or Not, Gemini Pro, Hive, Resemble.ai 4개였다. 오디오 검사가 가능한 7개 중에서는 Sensity와 Resemble.ai가 최상위였다 [Gigazine](https://gigazine.net/gsc_news/en/20260302-ai-detection-fake), [The Star](https://www.thestar.com.my/tech/tech-news/2026/03/10/these-tools-say-they-can-spot-ai-fakes-do-they-really-work).
5. **(독립 평가, 2차 검증 대상 아님)** Tow Center 테스트에서 범용 AI 챗봇 7종이 보도사진 10장의 출처 검증에 모두 실패했다 [CJR](https://www.cjr.org/tow_center/why-ai-models-are-bad-at-verifying-photos.php).
6. **(벤더 주장 대 독립 평가)** Intel FakeCatcher는 96%를 주장하지만, BBC 테스트에서는 진짜 영상을 여러 번 오탐했다 [PetaPixel](https://petapixel.com/2023/08/02/deepfake-detection-software-analyzes-a-persons-blood-flow).
7. **(정부 자체 발표, 확인)** 국과수·행안부 모델의 정확도가 76%에서 92%로 개선됐다(국소 분석과 전역 분석 앙상블, 2026-03-10 발표). 머니투데이는 '97%'를 제목으로 썼다. 선관위는 AND 규칙으로 운용한다 [세계일보](https://www.segye.com/newsView/20260310517457), [머니투데이](https://www.mt.co.kr/policy/2026/03/10/2026031015560960020), [뉴스1](https://www.news1.kr/amp/local/moi/6096576).
8. **(사례, 정정)** 김수현·김새론 녹취파일에 대한 국과수 '판정 불가'는 2025-11 강남경찰서에 회신됐다(보도 2025-12-15). 사유는 원본이 아니고 잡음이 많다는 것이었다. 이후 제보자가 최소 4가지 버전의 AI 녹음을 만든 정황이 보도됐다 [뉴데일리](https://www.newdaily.co.kr/site/data/html/2025/12/15/2025121500350.html), [다음(2026-06 후속)](https://v.daum.net/v/20260618090142444).
9. **(국책과제, 확인)** 경찰청 허위조작 콘텐츠 판별 시스템: 3년 91억 원, 연구기간 2025-04~2027-12. 숭실대가 음성, 성균관대가 영상·가짜뉴스, 연세대가 데이터셋, 부퍼탈대가 다국어 데이터, 한컴위드가 시스템·실증을 맡는다 [디지털데일리](https://www.ddaily.co.kr/page/view/2025020211334778803), [바이라인네트워크](https://byline.network/2025/06/5-299/).
10. **(법, 정정)** Rule 707: 2026-05-07 자문위원회가 원안과 재초안 3건 모두 재공고를 권고하지 않았고, 901(c)는 보류됐다. 2026-06-03~04 Standing Committee도 재검토로 돌려보냈고, 2026-10-15 보스턴에서 미니 컨퍼런스가 열렸다. 재초안은 범위를 'AI가 생성해 전문가 없이 제출된 증거'로 좁히고 사전 고지 요건을 추가했다. 시행은 빨라야 2029-12-01이다 [uscourts.gov](https://www.uscourts.gov/sites/default/files/document/advisory_committee_on_evidence_rules_may_2026.pdf), [Proskauer](https://www.proskauer.com/blog/machine-generated-evidence-challenges-the-federal-rules-inside-the-contested-proposed-federal-rule-of-evidence-707), [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence).
11. **(판례, 확인)** Mendones v. Cushman & Wakefield(Alameda 상급법원, 23CV028772, Kolakowski 판사, 2025-09-09): with prejudice 기각. 법원은 Exhibit 6C 증인 영상을 같은 인물이 나온 진짜 증거와 비교해 딥페이크로 판단했고, AI 탐지 점수는 근거가 아니었다. 1심이라 구속력 있는 선례는 아니다 [Volokh](https://reason.com/volokh/2025/09/25/court-throws-out-case-after-finding-plaintiffs-submitted-deepfake-videos-and-altered-images/), [NBC](https://www.nbcnews.com/tech/tech-news/ai-generated-evidence-deepfake-use-law-judges-object-rcna235976).
12. **(평가 프로그램, 확인)** NIST GenAI 이미지 판별 파일럿: 라운드3 결과 2026-04-10, 워크숍 2026-05. 공개 리더보드 수치는 2026-11 현재도 없다 [NIST](https://ai-challenges.nist.gov/t2i), [평가계획](https://ai-challenges.nist.gov/pub/GenAI_Image_Discriminators_Evalplan.pdf).
13. **(투자·M&A, 확인)** Reality Defender: Series A 3,300만 달러, 누적 4,390만~5,240만 달러, KPMG 소수 지분(2026-09-10) [PitchBook](https://pitchbook.com/profiles/company/491666-59), [Tracxn](https://tracxn.com/d/companies/reality-defender/__ZL3JQRZBSWQdBzjzHQ2Huwdcck9IR8XdS1G36uFDk3s). GetReal: Series A 1,750만 달러, 누적 2,450만 달러 [PitchBook](https://pitchbook.com/profiles/company/601967-53). Deel은 Clarity를 2026-08-03에 인수했다 [IDTechWire](https://idtechwire.com/deel-acquires-clarity-to-add-deepfake-detection-across-hiring-and-workforce-identity/).
14. **(벤더 입장)** Magnet은 '온라인 미디어에 대해 100% 신뢰할 수 있는 딥페이크 탐지 기술은 없다'고 밝혔다. Amped는 AI 탐지가 포렌식 해석을 대체하지 않는다고 명시한다 [Magnet](https://www.magnetforensics.com/blog/the-deepfake-detector-paradigm-shift-the-case-for-media-authentication-in-court/), [Amped 40960](https://blog.ampedsoftware.com/2026/06/25/authenticate-update-40960).

## 8. 검증에서 정정·삭제된 주요 사항

- **김수현 녹취 '판정 불가'.** 시점을 2026-06에서 2025-11 회신(2025-12 보도)으로 바로잡았다. 사유도 '음성 탐지 기술의 한계'에서 '원본 부재와 잡음'으로 정정했다. 이 사례는 탐지 정확도 문제보다 증거 보관 연속성과 출처 문제로 읽어야 한다.
- **Rule 707.** '2026-10 소위원회 구성'을 '2026-10-15 미니 컨퍼런스'로 바꿨다. 6월 Standing Committee 반려와 '빨라야 2029-12 시행' 분석을 추가했다.
- **Reality Defender.** 누적 투자 상한 6,600만 달러는 근거가 없어 4,000만~5,200만 달러로 바꿨다. KPMG 투자를 추가하고 실사용 점수를 3에서 3~4로 올렸다.
- **Hive.** 신뢰도를 4에서 3으로 내렸다. 우회 연구가 있고 부분 조작 탐지율이 27~73%이며, DIU 계약은 정확도 검증이 아니라 프로토타입 계약이다.
- **TrueMedia.** '클로즈드 베타 미확인'을 '클로즈드 베타 재출시(공식 사이트)'로 바꿨다.
- **Magnet.** AI 기능명을 'Magnet.AI'에서 'Magnet Copilot'(Axiom 8.0 얼리 액세스)으로 바꿨다. Medex 인수 시점 2024-08은 미확인이다.
- **경찰청 사업.** 시작 시점을 2025-02에서 연구기간 2025-04~2027-12로 바꿨다(2025-02는 보도 시점).
- **선관위 운용.** '다중 모델 교차검증'을 'AND 규칙(둘 다 딥페이크일 때만 확정)'으로 구체화했다.
- **점수 조정(편집자 판단).** Intel의 메이저성을 5에서 2로 내렸다(2023년 이후 활동 미확인). Sightengine의 신뢰도를 3에서 2로 내렸다(조작 탐지 33%). GetReal의 메이저성을 4에서 3으로, TrueMedia의 실사용을 3에서 2로 내렸다.
- **추가(missed).** Deel-Clarity 인수, KPMG-Reality Defender 투자, Gartner 딥페이크 탐지 쿼드런트(벤더 목록은 미확인), NYT 오디오 결과(Sensity, Resemble), Cellebrite 전용 탐지 기능 미확인, 김수현 사건 후속을 추가했다.
- **여전히 미확인.** Deepfake-Eval-2024 세부(상용 90% 미만, AUC 0.90 대 0.56, CVPRW 게재), NIST 결과 수치, 특허 장벽, AI FORCE 결과, Gartner 벤더 목록.
- **1차 요약본에서 뺀 것.** 근거가 약한 항목을 정리했다. Pindrop 행(검색 근거 없음), TAKE IT DOWN Act·EU AI Act·한국 AI 기본법 날짜(이번 검증에서 다루지 않음, 필요하면 다른 영역 요약본 참조), OpenAI 분류기 사례다.
