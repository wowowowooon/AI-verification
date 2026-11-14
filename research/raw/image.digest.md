# AI 생성·조작 이미지 탐지: 검증 반영 요약본 (2026-11-14 기준)

## 1. 영역 요약
- 빅테크(Google SynthID Detector, OpenAI Verify, Adobe)는 **자사·파트너 워터마크/C2PA 확인**을 무료로 제공한다. 범용 탐지기는 Hive가 기준점이고, Reality Defender·GetReal·Sensity·Pangram·AI or Not 등이 기업 시장에서 경쟁한다. [Google SynthID 공개](https://www.searchenginejournal.com/google-opens-synthid-watermark-detector-to-public/592226/) [Hive DoD 계약](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats)
- 수사·포렌식 시장에는 **Amped Authenticate, Magnet Verify/Axiom**이 이미 표준 도구로 자리 잡고 있다(조사 원본에서 누락됐던 내용). [Lexipol 가이드](https://www.lexipol.com/resources/blog/ai-generated-csam-after-anderegg/)
- 소비자 전용 앱은 미성숙하다. Google Play에서 확인된 최대 설치는 약 1.76만 건이다. [AppGoblin ForgeSpy](https://appgoblin.info/apps/io.zyur.forgespy)
- 독립 평가로 보면 최신 생성기, 후처리, 부분 조작 앞에서 신뢰도가 급락한다. 법정 증거 기준도 아직 정해지지 않았다. [arXiv 2602.07814](https://arxiv.org/html/2602.07814) [Proskauer FRE 707](https://www.proskauer.com/blog/machine-generated-evidence-challenges-the-federal-rules-inside-the-contested-proposed-federal-rule-of-evidence-707)
- 특허가 원천 봉쇄하는 영역은 없고, 기법 단위 특허와 C2PA 관련 KeeeX 소송(원고에게 불리하게 진행 중)만 있다.

## 2. 주요 제품 표 (중요도 순, 점수 1~5, 검증 반영)

| 제품 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| SynthID Detector + Gemini 검증 | Google(미국) | 웹·Gemini·Chrome·Search | 소비자·언론 | 5 | 5 | 3 | Gemini 2025.11.20, Detector 전 세계 공개 2026.10.7(영어). 이미지·영상·오디오(텍스트는 공개판 미포함) | 워터마크된 콘텐츠만 판별, '범용 탐지기 아님' 명시 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/) |
| Hive AI-Generated Content Detection | Hive(미국) | API·웹 데모·크롬 확장·온프레미스 | 플랫폼·정부·수사 | 5 | 4 | 3~4 | 운영중. DoD 240만 달러, DHS 15만 달러 시범계약 | UChicago 98.03%(교란 없는 AI 아트 기준) [arXiv 2402.03214](https://arxiv.org/pdf/2402.03214) |
| Amped Authenticate | Amped Software(이탈리아*) | 데스크톱 포렌식 SW | 수사기관 | 4 | 4 | 3 | 2026.3 확산모델 탐지 고도화, 이후 영상 딥페이크 추가 | 벤더 스스로 'AI 탐지는 증거가 아니라 선별용'이라고 명시 [Amped 블로그](https://blog.ampedsoftware.com/2026/03/11/authenticate-update-40165) |
| Magnet Verify / Axiom | Magnet Forensics(캐나다*) | 포렌식 플랫폼 | 수사·검찰·법률 | 4 | 4 | 3 | 운영중. '법정에서 설명·재현·방어 가능' 표방 | 100개 이상 데이터 포인트로 인증(벤더 주장) [Magnet](https://www.magnetforensics.com/blog/authenticity-on-trial-how-magnet-verify-helps-prosecutors-admit-digital-media-and-defeat-deepfake-defenses/) |
| Reality Defender | Reality Defender(미국) | 엔터프라이즈 플랫폼·API | 금융·정부 | 4 | 3 | 3 | 무료 티어 월 50건(영상 제외), 유료 월 399달러/1,000건. KPMG 소수지분 투자 2026.9.10 | 이미지 독립 평가 없음 [RD API](https://realitydefender.com/api) [KPMG](https://kpmg.com/us/en/media/news/kpmg-llp-takes-minority-stake-in-deepfake-detection-leader-reality-defender.html) |
| OpenAI Verify | OpenAI(미국) | 웹(프리뷰) | 소비자·언론 | 5 | 3 | 3 | 2026.5.19 공개. 이미지·오디오의 OpenAI 출처 신호만 확인 | 신호가 없다고 사람이 만든 것은 아님 [OpenAI 도움말](https://help.openai.com/en/articles/8912793-provenance-signals-content-credentials-synthid-in-openai-generated-content) |
| Adobe Content Authenticity | Adobe(미국) | 무료 웹·크롬 확장 | 크리에이터·언론 | 5 | 3 | 3 | 2025.4 베타, 2026.10 무료 웹앱 | C2PA 판독 전용, 메타데이터가 제거되면 판단 불가 [arXiv 2604.24890](https://arxiv.org/pdf/2604.24890) |
| AI or Not | AI or Not Inc.(미국) | 웹·API | 소비자·핀테크·KYC | 3 | 3 | 3 | 시드 500만 달러(2024.12~2025.1) | 사용자 수는 자기 진술뿐 [GamesBeat](https://gamesbeat.com/ai-or-not-raises-5m-to-stop-ai-fraud-deepfakes-and-misinformation/) |
| Sightengine | Sightengine(프랑스) | API·웹 데모 | 플랫폼·개발자 | 3 | 3 | 3 | 운영중. 월 29달러부터 | ARIA 98.3%는 원 논문에서 확인되지 않음 [ARIA 논문](https://www.arxiv.org/pdf/2404.14581) |
| GetReal Inspect | GetReal Security(미국) | 엔터프라이즈 | 보안·정부·포렌식 | 4 | 3 | 3 | 시리즈A 1,750만 달러(2025.3.26), 누적 2,450만 달러 | Hany Farid 공동창업, 공개 성능 데이터 없음 [GetReal 발표](https://www.getrealsecurity.com/resources/getreal-security-raises-17-5m-series-a-led-by-forgepoint-capital-to-address-rapidly-growing-threats-associated-with-generative-ai-and-malicious-digital-media) |
| Sensity AI | Sensity(네덜란드) | 플랫폼·API | 수사·포렌식·금융 | 3 | 3 | 3 | 2026.1 210만 달러, 2026.7 EIC 490만 유로 | 이미지 독립 평가 없음 [BiometricUpdate](https://www.biometricupdate.com/202607/sensity-ai-gets-eic-funding-for-forensics-focused-deepfake-detection-models) |
| Truepic | Truepic(미국) | SDK(촬영 시점 인증) | 보험·금융·미디어 | 4 | 3 | 3 | 운영중. KeeeX 소송 피고 | 이미 퍼진 이미지는 판별 불가 [Truepic](https://www.truepic.com/blog/content-provenance) |
| 딥브레인AI AI 디텍터 | 딥브레인AI(한국) | SaaS·API·경찰청 SW | 수사·공공·금융 | 3 | 3 | 3 | 경찰청 SW 누적 1,636건 활용(2026.8) | 탐지율 약 80%는 2024년 수치이고 현재 수치는 미공개 [뉴스핌](https://www.newspim.com/news/view/20260813000619) |
| Pangram Image | Pangram Labs(미국) | 웹·API | 기업·교육 | 3 | 2 | 2 | 2026.7 900만 달러와 함께 연구 프리뷰 공개. 2026.11.4 Image 1.0 출시는 미확인(재검증 실패) | 99.5%는 벤더 주장 [TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/) |
| ForgeSpy (소비자 앱 대표 사례) | Zyur(미확인) | Android·iOS 앱 | 소비자 | 1 | 2 | 2 | 2025.11 출시 | 약 1.76만 설치, MAU 약 2.7천(AppGoblin 추정) [AppGoblin](https://appgoblin.info/apps/io.zyur.forgespy) |

\* Amped·Magnet의 국가는 조사 원문에 출처가 없다. 일반적으로 알려진 본사 기준으로 적었으니 보고서에 쓰기 전에 확인이 필요하다.
기타: Resemble DETECT-3B(2025.12 1,300만 달러, 검증 단계에서 재확인 못함) [SiliconANGLE](https://siliconangle.com/2025/12/08/resemble-ai-hauls-13m-different-approach-deepfake-detection/). Copyleaks(2025.11.10 이미지 탐지 출시, 재확인 못함) [Axios](https://www.axios.com/2025/11/10/copyleaks-ai-detect-images). TruthScan(ZeroGPT·DeepAI에 라이선스, 탐지 회피 사업과 같은 계열) [Fortune PR](https://fortune.com/press-releases/zerogpt-truthscan-ai-image-detection-2026-01-22). Illuminarty(사람 그림 오탐 67.4%) [arXiv 2402.03214](https://arxiv.org/pdf/2402.03214).

## 3. 4개 기준 판정
**메이저성: 있다.** Google·OpenAI·Adobe가 무료 검증을 기본 기능으로 넣었다. 범용 탐지는 Hive, 수사 포렌식은 Amped·Magnet이 기준이다. [Google 블로그](https://blog.google/technology/ai/ai-image-verification-gemini-app/) [Amped](https://blog.ampedsoftware.com/2026/05/27/deepfake-forensics-workflow-for-image-analysis). 다만 빅테크 도구는 워터마크 확인기일 뿐 범용 탐지기가 아니다. Midjourney는 2026 중반까지 C2PA·워터마크를 넣지 않는다(2차 출처). [c2paviewer](https://c2paviewer.com/articles/ai-tools-c2pa-support)

**완성도·실사용: 소비자 앱은 낮고, 웹과 기본 기능은 높다.** 설치 10만 건 이상인 이미지 판별 전용 앱은 찾지 못했다. [AppBrain](https://www.appbrain.com/dev/Zyur/) AI or Not 사용자 약 33만 명은 CEO의 자기 진술이고 [DataInnovation](https://datainnovation.org/2025/08/5-qs-with-anatoly-kvitnitsky-ceo-of-ai-or-not/), 50만 명 이상은 제3자 표기라 확인되지 않았다. [CheckThat.ai](https://checkthat.ai/brands/ai-or-not) 수사 현장에서는 Amped·Magnet이 교육·조달 생태계와 함께 쓰인다. [ForensicFocus](https://www.forensicfocus.com/news/advanced-detection-tools-from-amped-software-aim-to-combat-ai-generated-csam-and-protect-children/)

**신뢰도: 범죄 수사 기준으로는 낮다.** 오픈소스 16종의 최고 평균 정확도는 75%였다(독립 평가, 제로샷 조건). [arXiv 2602.07814](https://arxiv.org/html/2602.07814) 상용 탐지기도 후처리 후 급락한다(Succinct, 벤더 수행). [Succinct](https://blog.succinct.xyz/ai-image-detection-benchmark/) Hive의 상위권 근거도 교란 없는 구형 생성기 기준이고, 교란을 넣으면 우회된다. [BiometricUpdate](https://www.biometricupdate.com/202412/dod-awards-contract-for-deepfake-detection-to-hive) 벤더(Amped)조차 '선별용'이라고 말한다.

**신규 진입 경쟁력: 범용으로는 낮고, 니치에서는 조건부로 있다.** 소비자 범용 앱은 무료 대체재와 기술 한계 때문에 수익화가 어렵다. 기업 API는 자금 격차가 크다(Hive 1,000건당 6달러, 제3자 스냅샷). [Hive 가격](https://thehive.ai/pricing) 수사급 시장에는 기존 포렌식 벤더가 있다. 반면 학습 데이터 정합성이 아키텍처보다 중요하다는 연구 결과는 특화 데이터(한국·문서 위조)로 승부하는 신규 진입자에게 유리하다. [arXiv 2602.07814](https://arxiv.org/html/2602.07814)

## 4. 레드오션 판정: **부분적**
- 범용 소비자 판별 앱은 **예(돈이 안 되는 포화 시장)**다. 저품질 앱이 난립하고, 빅테크 무료 검증이 있으며, 오탐률이 0~40%로 벌어진다. [EDMO/NewsGuard](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/)
- 기업·정부 API는 **레드오션에 진입하는 단계**다. 자금력 있는 기업들이 선점하고 있다. 다만 업계 통합은 아직이다. Deel-Clarity(2026.8)는 채용·본인확인용 영상·음성 탐지 인수일 뿐 이미지 시장 통합의 근거가 아니다. [TNW](https://thenextweb.com/news/deel-acquires-clarity-deepfake-detection) [Calcalist](https://www.calcalistech.com/ctechnews/article/bkeyex0sgl)
- 수사·포렌식은 **블루오션이 아니다(원본 판단 정정)**. Amped·Magnet이 조달 채널과 법정 실적을 쥐고 있다. 그래도 한국 환경, 문서 위조, 부분 조작 위치 표시는 미해결이다. [Magnet](https://www.magnetforensics.com/blog/tackling-deepfakes-lets-focus-on-authentication-not-detection/)
- 특허는 장벽이 되지 않는다. KeeeX 소송은 2026.3 항소법원이 비회원국 관할을 부정했고, 정정 신청을 기각했으며, 원고에게 20만 유로 담보 제공을 명령했다. [UPC 명령](https://www.unifiedpatentcourt.org/sites/default/files/files/api_order/922-2026%20Adobe%20ea%20Final%20Order%20en-GB.pdf) [Wolters Kluwer](https://legalblogs.wolterskluwer.com/patent-blog/keeexed-out-the-upcs-long-arm-stops-at-the-line/)

## 5. 빈틈·기회 (출처는 조사 원본 근거)
- **통합 검증 리포트**: C2PA, SynthID·OpenAI Verify, 자체 탐지, 역검색, EXIF를 한 화면에 모으는 도구가 없다. 2027.1.1부터 캘리포니아 대형 플랫폼에 프로비넌스 탐지·표시 의무가 생기므로 B2B 검증 API 수요의 근거가 된다. [Morgan Lewis](https://www.morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative) [AB 853](https://app.legiplex.com/ca/legislature/2025/2025-r/bills/ab853)
- **부분 합성·인페인팅 위치 표시**: 상용 도구가 가장 약한 영역이다. Copyleaks가 이제 막 시작했다(벤더 주장: 혼합 이미지 조작 영역 40% 이상 식별). [Copyleaks 방법론](https://copyleaks.com/ai-image-detector/testing-methodology)
- **문서·영수증·신분증 위조**: GPT-Image-2 텍스트 이미지 벤치마크에서 탐지기들이 무너졌다. [HF 2606.19259](https://huggingface.co/papers/2606.19259.md) AI or Not도 KYC 쪽으로 포지셔닝을 강화하는 중이다. [CheckThat.ai](https://checkthat.ai/brands/ai-or-not)
- **한국 특화**: 한국인 얼굴, 한글, 메신저 재압축 경로에 맞춘 데이터. 딥브레인AI가 한국인 데이터 100만 건을 선례로 내세운다. [딥브레인AI](https://www.aistudios.com/ko/deepfake-detecting) 경찰청의 '탐지·판독·포렌식 3중 대응체계'와 2026.1~7월 딥페이크 피의자 419명 검거(17명 구속)는 B2G 수요가 커지는 신호다. [파이낸셜뉴스](https://www.fnnews.com/news/202608131007468569)
- **워터마크 미삽입 생성기 대응**(Midjourney, 오픈소스 Flux 계열): 빅테크 검증이 닿지 않는 사각지대다. [c2paviewer](https://c2paviewer.com/articles/ai-tools-c2pa-support)
- **재현성·검증을 문서화한 수사 보조 리포트**: 미국에는 AI 증거 전용 규칙이 없어 Rule 702 전문가 증언 체계에 기대야 한다. 기존 포렌식 벤더(Amped·Magnet)와 경쟁하기보다 연동하거나 보완하는 쪽이 현실적이다. [CaseRead](https://www.caseread.ai/blog/fre-707-ai-generated-evidence)
- **공개 벤치마크·오탐률 공시와 빠른 재학습 파이프라인**: 대부분의 경쟁사는 독립 수치를 공개하지 않는다. [Reality Defender 보도](https://www.securitysystemsnews.com/article/reality-defender-launches-public-api-and-free-tier)

## 6. 위협·장벽
- **무료 대체재**: Google, OpenAI, Adobe. 법적 의무는 캘리포니아 SB 942/AB 853에만 있다(월 사용자 100만 이상 생성 서비스에 무료 탐지 도구 제공). 이 기준도 계류 중인 SB 1000에 따라 바뀔 수 있다. **EU AI Act는 무료 탐지 도구를 의무화하지 않는다.** [Morgan Lewis](https://www.morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative) [CSA](https://labs.cloudsecurityalliance.org/research/csa-research-note-eu-ai-act-article50-watermarking-deadline/)
- **군비경쟁·회피**: 후처리, 적대적 교란, 워터마크 제거 공격(MarkNull로 SynthID-Image 100% 제거)이 있다. [arXiv 2608.10166](https://arxiv.org/pdf/2608.10166)
- **오탐의 법적 위험**: NewsGuard 평균 오탐 13.3%(실제 사진 15장, 표본이 작음), Full Fact가 확인한 SynthID 오탐 사례. [NewsGuard 2차](https://www.photoworkout.com/ai-detectors-false-positives-no-appeal/) [Full Fact](https://fullfact.org/toolkit/google-synthid-detector-flagging-apparently-real-images/)
- **운영비**: TrueMedia.org는 2025.1 종료했고, Georgetown이 이관받아 클로즈드 베타(대기자 명단제)로만 운영한다. [GeekWire](https://www.geekwire.com/2025/truemedia-is-back-deepfake-detection-tool-revived-now-managed-by-georgetown-university/) [Georgetown](https://mccourt.georgetown.edu/news/truemedia-finds-new-home-at-georgetowns-mccourt-school/)
- **수사 시장 기존 강자와 조달 장벽**: Amped·Magnet, 그리고 DoD·DHS-Hive, 경찰청-딥브레인AI 계약이 있다. [DHS 계약](https://dataconomy.com/2025/09/29/dhs-uses-ai-to-detect-ai-generated-child-abuse-material/)
- **자금 격차**: Hive 2021 기업가치 20억 달러(확정). 2026.5 시리즈E(31.6억 달러) 보도는 미확인이다. [SiliconANGLE](https://siliconangle.com/2021/04/21/enterprise-ai-solutions-startup-hive-raises-85m-2b-valuation/) [Forge](https://forgeglobal.com/hive-ai_stock/)
- **데이터·법 제약**: 성착취물은 학습할 수 없고, 얼굴 개인정보를 다뤄야 한다. 한국 AI 기본법 과태료 상한 3,000만 원은 시정명령 불이행 시에 해당하며, 계도기간이 최소 1년이라 실제 부과는 2027년 이후다. [머니투데이](https://www.mt.co.kr/tech/2025/12/31/2025123009504430416)

## 7. 핵심 사실 목록
- Hive: DIU 2년 240만 달러 계약(2024.12.5, 36개 지원사 중 선정, 오프라인 배포). [BusinessWire](https://www.businesswire.com/news/home/20241205852015/en/Hive-Secures-DoD-Contract-for-Deepfake-Detection-Pioneering-AI-Defense-Against-Emerging-Threats)
- Hive: DHS 사이버범죄센터 AI 생성 아동성착취물 판별 시범계약 15만 달러, 3개월, 수의계약. 수의계약 근거가 UChicago 연구와 DoD 계약이라 근거가 순환한다. [getcoai](https://getcoai.com/news/dhs-deploys-ai-tools-to-detect-fake-child-abuse-imagery)
- 독립 평가: UChicago(ACM CCS)에서 Hive 정확도 98.03%, 오탐 0%, 미탐 3.17%(교란 없는 AI 아트). AI or Not(당시 Optic)은 사람 그림 오탐 24.47%, Illuminarty 67.4%. [arXiv 2402.03214](https://arxiv.org/pdf/2402.03214)
- 독립 평가: 오픈소스 16종(260만 장, 생성기 291종) 최고 평균 75%, 최저 37.5%. Midjourney v7·Flux Dev·Firefly v4 탐지율 18~30%. [arXiv 2602.07814](https://arxiv.org/html/2602.07814)
- 벤더 수행 평가: Succinct(7개 상용 탐지기, 15,630장)에서 후처리 후 탐지율 급락, 헤드라인은 '최저 4%'. 탐지기별 98/90/90에서 36/11/13으로의 하락은 원 표로 확인하지 못했다. [Succinct](https://aidetection.succinct.xyz)
- 독립 평가: NewsGuard(2026.4말~5초) 실제 사진 15장 평균 오탐 13.3%, ScamAI 40%. 도구별 수치(Hive·Sightengine 0%, AI or Not 6.67%, Sightengine 대폭 조작 5/15)는 2차 보도로만 확인됐다. [EDMO](https://edmo.eu/publications/major-ai-image-detection-tools-deceive-online-users-often-classifying-authentic-images-as-fakes/)
- 벤더 주장: AI or Not 98.9% [AI or Not API](https://detection.aiornot.com/ai-image-detector-api/). Pangram 99.5% [TechCrunch](https://techcrunch.com/2026/07/29/as-ai-content-floods-the-internet-pangram-raises-9m-to-detect-it/). 딥브레인AI 90% 이상 [딥브레인AI](https://www.aistudios.com/ko/deepfake-detecting). Copyleaks 95% 이상 [Copyleaks](https://copyleaks.com/blog/introducing-copyleaks-ai-image-detection). Sightengine ARIA 98.3%(재검증 못함) [Sightengine](https://sightengine.com/best-ai-image-detectors-benchmark).
- 가격: Hive 1,000건당 6달러(pricingsaas 스냅샷, 원문은 확인 못함), 결제수단 등록 시 50달러 이상 무료 크레딧, 하루 100건 기본 한도. Reality Defender 무료 월 50건, 유료 월 399달러/1,000건. Sightengine 월 29달러/1만 operation. [Hive 가격](https://thehive.ai/pricing) [RD API](https://realitydefender.com/api) [Sightengine 가격](https://sightengine.com/pricing)
- Google SynthID Detector 2026.10.7 전 세계 공개. 파트너는 OpenAI·NVIDIA·Kakao, Apple은 예정. 'AI 생성과 AI 편집을 구분하지 못한다'고 밝힘. [MacRumors](https://www.macrumors.com/2026/10/07/google-synthid-detector/)
- 한국 경찰청: 탐지 SW 누적 1,636건 활용(2026 선거범죄 72건 포함, 2026.8.13 발표). 탐지율 약 80%는 2024.3 공개 당시 수치다. [뉴스핌](https://www.newspim.com/news/view/20260813000619) [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364)
- 규제: 한국 AI 기본법 2026.1.22 시행 [뉴시스](https://www.newsis.com/view/NISX20260122_0003486463). EU 제50조는 2026.8.2 시행했고, Digital Omnibus(2026.6.29 승인)로 제50(2)조 워터마킹은 기존 출시 시스템에 한해 2026.12.2까지 유예됐다 [Winston Taylor](https://www.winstontaylor.com/insights/ai-act-rules-on-high-risk-ai-delayed-as-ai-digital-omnibus-agreed). 캘리포니아는 2028.1.1부터 촬영기기 기본 공시 의무 [Morgan Lewis](https://www.morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative).
- 미국 증거규칙: FRE 707은 2026.5 자문위원회에서 미승인됐고, 2026.10.15 707·901(c) 미니 컨퍼런스가 열렸다. 가장 빠른 시행 전망은 2029.12. [Proskauer](https://www.proskauer.com/blog/machine-generated-evidence-challenges-the-federal-rules-inside-the-contested-proposed-federal-rule-of-evidence-707) [TrueScreen](https://truescreen.io/articles/federal-rule-707-ai-generated-evidence/)
- 시장 규모: 2025년 약 7억~12억 달러, 연평균 성장률 25~37%(보고서마다 다르고 신뢰도 낮음). [SNS Insider](https://www.snsinsider.com/reports/deepfake-detection-market-11090)

## 8. 검증에서 정정·삭제된 주요 사항
- **누락 보완**: Amped Authenticate와 Magnet Verify/Axiom을 추가했다. 그에 따라 '수사급 포렌식은 블루오션 성격'이라는 판단을 '기존 벤더가 있는 시장'으로 정정했다.
- **EU AI Act**: '무료 탐지 도구 의무화'를 삭제했다. 이는 캘리포니아에만 있는 의무다. 제50(2)조 유예(2026.12.2)와 캘리포니아 2027 플랫폼 탐지 의무를 추가했다.
- **Hive**: 신뢰도를 4에서 3~4로 낮췄다(구형 생성기 기준 근거, 교란 취약성, 근거 순환). 단가는 0.003달러에서 0.006달러로 바로잡았다. 시리즈E는 미확인으로 표시했다.
- **AI or Not**: 사용자 수 신뢰도를 high에서 낮음으로 바꿨다(자기 진술·제3자 표기). 실사용 점수를 4에서 3으로 낮췄다.
- **Reality Defender**: '반론 보도'(Crypto Briefing)를 삭제했다. KPMG 투자는 공식 확정으로 바꿨다. 누적 투자는 3,300만~5,240만 달러로 트래커마다 다르다고 적었다.
- **Google SynthID Detector**: 대상 매체에서 텍스트를 뺐다. **OpenAI Verify**: '이미지만'을 '이미지·오디오'로 정정했다.
- **경찰청 80%**: 2024년 수치임을 밝히고 1,636건(2026.8)과 분리해 적었다.
- **KeeeX 소송**: 원고에게 불리한 2026.3 항소법원 결정을 추가했다. 특허 리스크 판단을 '더 낮음'으로 강화했다.
- **Deel-Clarity**: '이미지 탐지 시장 통합' 근거로 쓴 부분을 삭제했다(영상·음성 KYC 회사 인수임).
- **TrueMedia**: 재가동은 클로즈드 베타(이미지·오디오)라고 정정했다.
- **NewsGuard·Succinct·arXiv 2602.07814**: NewsGuard는 표본이 작고, Succinct는 벤더가 수행했으며, arXiv 논문은 제로샷 조건이라는 한계를 명시했다. confidence high에서 낮췄다.
- **미확인으로 남은 항목**: Pangram Image 1.0(2026.11.4), Copyleaks 출시 내용, Resemble 1,300만 달러, Sightengine ARIA 98.3%, ForgeSpy 설치 수. 이들은 웹 검색 한도 때문에 재검증하지 못했다. newsguardtech.com과 pricingsaas.com 원문은 네트워크 제한으로 열지 못했다.
