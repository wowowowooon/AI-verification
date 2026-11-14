# 빅테크·표준 기반 출처증명/워터마크와 규제: 검증 반영 요약본

기준일 2026-11-14. 원 조사는 WebSearch 37회, 팩트체크는 18회를 썼고 WebFetch는 둘 다 쓰지 않았다. 근거는 주로 2차 보도와 로펌 분석이다. 팩트체크가 독립적으로 확인하지 못한 항목(Gemini MAU, Lead Stories 테스트, Nikon 복구 상태, Microsoft 보고서 세부, 중국 집행 수치, 선관위 8,832건, Galaxy S26 라벨, Amazon·Truepic 현황)은 원 조사 서술을 그대로 옮겼다. 검증 결과는 확인 11건, 정정 6건, 반박 0건이다.

## 1. 영역 요약

- 구글 SynthID가 사실상 업계 공용 워터마크가 됐다. 여기에 OpenAI, NVIDIA, Kakao, ElevenLabs가 참여했고 Apple은 예정이다. 확인 기능은 Search, Chrome, Gemini에 무료로 기본 탑재됐다. Google은 기업용 탐지 API도 프리뷰로 팔기 시작했다.
- C2PA는 로열티 프리 표준이다. Pixel 10, Galaxy, 카메라를 거쳐 퍼졌지만, 업로드하면 메타데이터가 지워지고 기기 구현에 결함이 있어 신뢰도가 낮다.
- 생태계는 쪼개져 있다. Meta, Microsoft, TikTok은 각자 자체 워터마크를 쓰고, Apple은 C2PA가 아닌 Reference Image를 내놓았다.
- 독립 검증 결과는 대체로 부정적이다(Meta 탐지기 55% 미탐, Gemini 판정 비일관성). 오픈웨이트 모델 산출물은 처음부터 워터마크 체계 밖에 있다.
- 규제는 한국 AI 기본법, EU 50조, 캘리포니아 SB 942/AB 853/SB 1000, TAKE IT DOWN, 중국 표시 규정이 동시에 시행 중이다. 이 규제들이 표시·검증·삭제 수요를 만든다.

## 2. 주요 제품 표 (점수 1~5, 검증 반영)

| 제품 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| SynthID Detector 포털 | Google DeepMind(미국) | 무료 웹 포털 | 소비자·언론 | 5 | 3(추정) | 3 | 2026-10-07 전 세계 공개(영어) | 협조사 워터마크만 '검출/미검출'로 판정, 오류율 비공개 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/) |
| Search·Chrome·Circle to Search 확인 | Google(미국) | 검색·브라우저 기본 기능 | 소비자 | 5 | 4 | 3 | SynthID 2026-05~ 배포, C2PA는 예정 | 수십억 명에게 기본 노출 [Google I/O](https://blog.google/innovation-and-ai/technology/ai/io-2026-keynote-moment-videos/) |
| Gemini 앱 확인 기능 | Google(미국) | 앱 기능 | 소비자 | 5 | 4 | 2 | 이미지 2025-11, 영상 2025-12, C2PA 2026 | 한 대화 안에서 판정이 엇갈림(팩트체크 미확인) [Lead Stories](https://leadstories.com/analysis/2026/07/google-gemini-synthid-detector-confuses-results-within-same-chat.html) |
| Google Cloud AI Content Detection API | Google(미국) | 기업용 API | 기업 | 5 | 2 | 미확인 | 2026-05 신뢰 파트너 대상 프리뷰 | Shutterstock·Snap·Fox Sports·Canva에 제공 [InfoQ](https://infoq.com/news/2026/05/google-synthid-content-detection) |
| YouTube 자동 AI 라벨 + 초상 탐지 | Google(미국) | 플랫폼 기능 | 소비자·크리에이터 | 5 | 5 | 2 | 2026-05 자동 라벨, 성인 크리에이터 전원에게 개방 | 정확도 비공개 [MBW](https://www.musicbusinessworldwide.com/youtube-will-now-automatically-detect-and-label-ai-videos-even-when-creators-dont-disclose-it/) |
| TikTok AIGC 라벨 + 비가시 워터마크 | ByteDance(중국) | 플랫폼 기능 | 소비자 | 5 | 5 | 2 | 2025-11 워터마크 테스트 | 워터마크는 TikTok 내부에서만 읽힘 [TechCrunch](https://techcrunch.com/2025/11/18/tiktok-now-lets-you-choose-how-much-ai-generated-content-you-want-to-see/) |
| Meta AI info 라벨 + Content Seal | Meta(미국) | 플랫폼 라벨 + 탐지 프리뷰 | 소비자 | 5 | 4 | 1 | 2026-07 프리뷰 | 자르기만 해도 55% 미탐(Reuters) [The Star](https://www.thestar.com.my/tech/tech-news/2026/07/10/meta-ai-image-detector-fails-to-identify-some-of-its-own-cropped-ai-images-reuters-analysis-finds) |
| OpenAI Verify | OpenAI(미국) | 웹 도구(Research preview) | 일반·개발자 | 5 | 2 | 2 | 이미지 2026-05-19, 오디오 확대(범위 엇갈림) | 자사 산출물 전용, 대량 검증 API 여부 불분명 [OpenAI 도움말](https://help.openai.com/en/articles/8912793-c2pa-in-chatgpt-images) |
| C2PA Verify / SDK / 적합성 프로그램 | C2PA·CAI(국제) | 오픈 표준·SDK | 언론·개발자 | 5 | 3 | 2 | 31개사 54개 제품 통과(2026-05) | 로열티 프리, 메타데이터 제거에 취약 [C2PA FAQ](https://www.c2pa.org/faq) |
| Adobe Content Authenticity | Adobe(미국) | 웹 앱 + Chrome 확장 | 크리에이터·언론 | 5 | 3 | 2 | 퍼블릭 베타, GA 미확인 | 자격증명이 붙은 콘텐츠만 의미가 있음 [Adobe](https://helpx.adobe.com/ae_en/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html) |
| Pixel 10 Content Credentials | Google(미국) | 온디바이스 서명 | 소비자 | 5 | 3 | 3 | 모든 JPEG 서명, AL2(벤더 주장) | 진본 증명 기능이지 탐지기가 아님 [Google Security](https://security.googleblog.com/2025/09/pixel-android-trusted-images-c2pa-content-credentials.html) |
| Galaxy S25/S26 AI 편집 라벨 | Samsung(한국) | 온디바이스 | 소비자 | 5 | 4 | 2 | AI 편집물에만 C2PA 부착 | exiftool로 쉽게 제거, '거꾸로 된 접근' 비판 [PetaPixel](https://petapixel.com/2025/02/13/samsungs-image-authenticity-approach-is-backward-and-its-ais-fault) |
| Apple Reference Image | Apple(미국) | 온디바이스 센서 서명 | 소비자·언론 | 5 | 2 | 3 | 2026-09 iPhone 18 Pro, 사용자가 켜는 모드 | C2PA 아님, 48MP 메인 카메라 한정 [Nieman Lab](https://www.niemanlab.org/2026/09/apple-launches-a-new-way-to-prove-a-photo-was-shot-with-an-iphone-not-generated-by-ai/) |
| ElevenLabs Audio Detector | ElevenLabs(미국) | 무료 웹 도구 | 일반·언론 | 4 | 3 | 3 | 2026-07 SynthID 적용 | 자사 오디오만 판정 [ElevenLabs](https://elevenlabs.io/blog/synthid) |
| Microsoft Paint·Photos 워터마크 + C2PA | Microsoft(미국) | 생성물 삽입 | 기업·소비자 | 5 | 2 | 2 | 운영중 | SynthID와 호환되지 않음, 자사 보고서도 단일 방법은 불충분하다고 결론 [arXiv 2602.18681](https://arxiv.org/abs/2602.18681) |

표에서 뺀 항목: Nikon Z6III는 위조 서명 취약점으로 인증서를 전량 폐기했고 2026-05까지 복구되지 않았다(팩트체크 미확인) [DCW](https://www.digitalcameraworld.com/photography/photojournalism/nikon-revokes-all-c2pa-image-authenticity-certificates-after-major-vulnerability-exposed). OpenAI 텍스트 분류기는 2023-07 종료됐다. 벤더 자체 평가로 AI 글의 26%만 식별하고 사람 글의 9%를 오탐했다. 미확인(사전 지식) [OpenAI](https://openai.com/index/new-ai-classifier-for-indicating-ai-written-text/). Amazon Bedrock 워터마크 탐지와 Truepic은 미확인(사전 지식)이다.

## 3. 4개 기준 판정

**메이저성: 매우 높음.** Google, OpenAI, Meta, Microsoft, Apple, Samsung, TikTok, Adobe가 모두 직접 뛰어들었다. SynthID 연합에는 OpenAI, NVIDIA, Kakao, ElevenLabs가 있고 Apple이 예정돼 있다 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/). Google은 소비자 포털과 기업용 API를 모두 갖췄다 [InfoQ](https://infoq.com/news/2026/05/google-synthid-content-detection).

**완성도·실사용: 배포 채널은 압도적이지만 이용 지표는 없다.** 확인 기능은 Search, Chrome, Gemini, YouTube, TikTok에 기본으로 들어가 있다. 그러나 포털이나 검증 도구의 이용자 수는 어느 회사도 공개하지 않는다. SynthID Detector는 영어만 지원하고, OpenAI Verify는 아직 Research preview다 [OpenAI 도움말](https://help.openai.com/en/articles/8912793-c2pa-in-chatgpt-images).

**신뢰도: 낮음~중간.** 벤더 주장은 '자르기·압축에 견고하다'는 것이지만 정량 오류율은 공개하지 않는다. 독립 평가는 다음과 같다.
- Meta 탐지기는 자르기만 해도 55%를 놓쳤다. 표본은 40장이다 [Cybernews](https://cybernews.com/ai-news/metas-ai-detector-misses-some-cropped-images/).
- SynthID는 재생성 공격에 무력하다 [AI Weekly](https://aiweekly.co/alerts/google-synthid-watermarks-hold-up-in-tests-labeling-still-slips).
- 텍스트 워터마크는 패러프레이즈만으로 98.3%가 제거된다. 재현되지 않은 프리프린트다 [arXiv 2607.16010](https://arxiv.org/abs/2607.16010).
- 워터마크 '미검출'은 사람이 만들었다는 증거가 아니라고 각 사가 스스로 밝힌다.

**신규 진입 경쟁력: 출처증명 레이어에서는 없음. 사후 탐지·통합·포렌식 레이어에서는 조건부.** 워터마크와 C2PA를 소규모 팀이 직접 만드는 것은 무의미하다. 기회는 두 곳에 있다. 하나는 SB 1000의 제3자 검증도구 조항과 EU 상호운용성 기한이 만드는 통합 검증 B2B다. 다른 하나는 워터마크가 없는 콘텐츠의 포렌식이다. 다만 B2B에서는 Google 기업용 API가, B2G에서는 경찰청 자체 도구가 이미 경쟁자로 있다.

## 4. 레드오션 판정: 부분적

- **예(레드오션을 넘어 무료 기능에 흡수됨):** "주요 생성기로 만든 콘텐츠인지 확인하는" B2C 앱이 여기에 해당한다. SynthID 연합의 무료 포털이 있고, Search·Chrome·Gemini에 기본 탑재됐고, 플랫폼 자동 라벨이 붙는다. 캘리포니아 법은 생성 AI 제공자에게 검증도구 제공을 의무화했다 [Morgan Lewis](https://morganlewis.com/pubs/2026/08/new-california-ai-disclosure-rules-become-operative).
- **아니오(빈 영역이지만 블루오션은 아님):** 워터마크가 없거나 지워진 콘텐츠의 사후 탐지와 법정 증거용 포렌식이 여기에 해당한다. 대상은 오픈웨이트 모델(Wan 2.x 등) 산출물 [arXiv 2512.11815](https://arxiv.org/abs/2512.11815v2), 업로드 때 메타데이터가 지워진 콘텐츠, 재생성 공격을 받은 콘텐츠다. 다만 실전 성능이 크게 떨어진다. Deepfake-Eval-2024에서 AUC가 45~50% 하락했다 [HF Papers](https://huggingface.co/papers/2503.02857). 여기에 경찰 내부 도구와 Google API도 경쟁자다.
- **특허:** C2PA는 로열티 프리라 통합 리스크가 낮다 [C2PA FAQ](https://www.c2pa.org/faq). SynthID 특허와 라이선스 조건, 사후 탐지 전반의 FTO는 미확인이다.

## 5. 빈틈·기회

1. **워터마크 제거 흔적 탐지:** 제거 처리 이미지를 오탐률 1% 기준에서 98% 넘게 잡아냈다 [arXiv 2605.09203](https://arxiv.org/pdf/2605.09203). 이를 이용하면 '없음'을 '원래 없음'과 '지워짐'으로 나눌 수 있다. 단, 동료 심사를 거치지 않은 프리프린트다. 평가한 제거 도구의 제거 성공률부터 1.1~66.8%로 편차가 크고, 처음 보는 제거 도구에 일반화되는지는 검증되지 않았다(confidence: medium~low).
2. **쪼개진 출처 신호의 통합 검증 + 사후 탐지 하이브리드:** SynthID, Content Seal, Microsoft 워터마크, C2PA, Apple Reference Image를 한 번에 확인하는 도구다. EU 실천강령 서명사는 2027-02-02까지 워터마크 탐지 상호운용성을 구현해야 하고, 2026-07-31 기준 서명 조직은 약 190곳이다 [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/technology-quotient/eu-ai-act-unpacked-33-the-final-code-of-practice-on-transparency-of-ai-generate-102n4yx). 대형 서명사들이 직접 구현하면 이 기회는 흡수될 수 있다.
3. **캘리포니아 SB 1000 화이트라벨 검증도구:** 100만 명 기준이 사라져 모든 생성 AI 제공자가 대상이 됐다. 이들은 '자격을 갖춘 제3자 검증도구'로 안내해도 의무를 이행할 수 있다. 지원해야 하는 것은 잠재 표시뿐이고, 검증도구는 개인정보를 동의 없이 내보내면 안 된다 [Latham](https://www.lw.com/en/insights/newest-slate-of-ai-laws-keeps-california-at-the-forefront-of-us-regulation), [Sheppard](https://www.sheppard.com/insights/blogs/california-enacts-ai-spokespeople-chatbots-and-content-disclosures-laws).
4. **법정 증거용 포렌식 리포트:** 오류율 공개, 재현성, 처리 이력(chain of custody), 근거 시각화를 갖춘 리포트다. 빅테크는 오류율조차 공개하지 않는다 [arXiv 2602.18681](https://arxiv.org/abs/2602.18681).
5. **한국 B2G·B2B:** 경찰 집행(7개월 동안 419명 검거) [M이코노미](https://www.m-economynews.com/mobile/article.html?no=69729), 선관위 딥페이크 삭제 요청 8,832건 [코리아데일리](https://www.koreadaily.com/article/20260521130058516), 방미통위의 유통방지 대상 이미지 확대 [뉴시스](https://mobile.newsis.com/view/NISX20260721_0003716596)가 수요 근거다.
6. **오디오(보이스피싱)와 한국어 특화:** YouTube 음성복제 탐지는 2026년 후반 예정이고, ElevenLabs 탐지기는 자사 음성만 판정한다. 비교 평가는 미확인이다.
7. **덴마크 법안 L 49:** 게시자에게 입증 책임을 지운다. 아직 통과되지 않았다. 통과되면 출처 증명 수요가 생길 수 있다 [Euronews](https://www.euronews.com/2026/10/08/denmark-introduces-a-bill-protecting-peoples-faces-and-voices-from-deepfakes).

## 6. 위협·장벽

- **B2C 무료화:** SynthID 연합의 무료 포털이 있고, Search·Chrome·Gemini에 기본 탑재됐다.
- **Google의 B2B 진입:** 기업용 AI Content Detection API가 2026-05부터 프리뷰 중이다 [InfoQ](https://infoq.com/news/2026/05/google-synthid-content-detection).
- **플랫폼 자체 탐지:** YouTube, TikTok, Meta가 플랫폼 안에서 직접 탐지하고 라벨을 붙인다.
- **기존 B2G 공급자:** 경찰청은 2024년에 탐지 SW를 자체 개발했다. 당시 정확도는 약 80%로 수사 참고용이었고, 지금까지 수사 1,636건에 쓰였으며 선거범죄 등으로 범위를 넓혔다 [보안뉴스](https://m.boannews.com/html/detail.html?idx=127364). 행안부·국과수가 선관위에 탐지 도구를 제공했다는 보도도 있다 [세계일보](https://www.segye.com/newsView/20260310517457).
- **기술 난도와 오탐 책임:** 실전에서 AUC가 45~50% 떨어지고 [HF Papers](https://huggingface.co/papers/2503.02857), 오탐은 명예훼손이나 부당 수사로 이어질 수 있다.
- **텍스트가 가장 약함:** 텍스트 워터마크는 패러프레이즈로 제거되고, OpenAI는 텍스트 분류기를 철수했다.
- **약관 제약:** OpenAI 약관은 워터마크를 역공학하려는 반복 질의를 금지한다 [OpenAI](https://openai.com/index/advancing-content-provenance).
- **규제 일정 불확실:** 한국은 과태료 부과가 2027년 이후다. EU 옴니버스는 관보 게재를 확인하지 못했다. 미국은 연방 행정명령이 주법을 견제한다 [Ropes & Gray](https://www.ropesgray.com/en/insights/alerts/2025/12/trump-attempts-to-preempt-state-ai-regulation-through-executive-order).

## 7. 핵심 사실 목록

- SynthID Detector는 2026-10-07 전 세계 공개(영어). OpenAI·NVIDIA·Kakao를 지원하고 Apple은 '곧'(날짜 미공개). 포털 주소는 synthid.com과 synthid.google 가운데 어느 쪽이 현재 주소인지 미확인 [eWeek](https://www.eweek.com/news/googles-synthid-detector-goes-public-with-openai-and-nvidia-support/), [Mixed](https://mixed-news.com/en/google-synthid-detector-worldwide-apple-ai-content-comes-soon/)
- 벤더 주장: 구글은 이미지·영상 1천억 건 이상과 오디오 6만 년 분량에 SynthID를 넣었다(2차 보도) [InfoQ](https://infoq.com/news/2026/10/synthid-watermarking-detector)
- OpenAI는 2026-05-19부터 ChatGPT·Codex·API 이미지에 C2PA와 SynthID를 함께 넣는다. Verify는 Research preview [OpenAI](https://openai.com/index/advancing-content-provenance)
- Kakao는 2026-05-20 SynthID 도입을 발표했다. 대상은 카나나 콜라주(이미지), 카나나 키네마(영상), 카카오톡 카나나 템플릿이며 실제 적용 여부는 미확인 [카카오](https://www.kakaocorp.com/page/detail/12039?lang=KOR)
- ElevenLabs는 2026-07 전체 오디오에 SynthID를 적용했다 [ElevenLabs](https://elevenlabs.io/blog/synthid)
- OpenAI는 2026-03-24 Sora 앱·API 종료를 발표했다. 앱은 2026-04-26, API는 2026-09-24 종료(단일 출처) [Engadget](https://engadget.com/ai/openai-is-shutting-down-its-sora-video-generation-app-211023358.html), [The Decoder](https://the-decoder.com/openai-sets-two-stage-sora-shutdown-with-app-closing-april-2026-and-api-following-in-september/)
- 독립 평가: Washington Post가 C2PA가 든 Sora 영상을 8개 플랫폼에 올렸더니 모두 자격증명을 보존·표시하지 않았다(2025-10 테스트) [AIID](https://incidentdatabase.ai/reports/6301)
- 독립 평가: Reuters 분석에서 Meta 탐지기는 원본 40장을 모두 잡았고, 잘린 이미지는 55%를 놓쳤다(2026-07-10) [Gizmodo](https://gizmodo.com/metas-ai-detector-cant-detect-images-it-generated-itself-report-finds-2000784335)
- 독립 평가: SynthID-Text는 패러프레이즈로 98.3%(조건부)가 제거되고 사람 글 오탐률은 5.4%였다. MarkLLM 구현으로 실험했고 'Daubert 미충족'은 저자의 평가다 [arXiv 2607.16010](https://arxiv.org/abs/2607.16010)
- Microsoft 보고서(2026-02): 단일 기술로는 믿을 만하게 구별할 수 없고, '역전 공격' 위험이 있다 [The Decoder](https://the-decoder.com/microsofts-research-argues-ai-media-authentication-doesnt-work-reliably-yet-new-laws-assume-it-does/)
- C2PA 적합성 프로그램: 31개사 54개 제품 통과(2026-05-14) [CAI](https://opensource.contentauthenticity.org/docs/conformance/)
- Apple Reference Image: 사용자가 켜는 모드이고 48MP 메인 카메라에서만 작동한다. 검증 API는 Apple 플랫폼 전용 [IEEE Spectrum](https://spectrum.ieee.org/apple-reference-image)
- 한국 AI 기본법(2026-01-22 시행): 표시 의무는 사업자에게만 있다. 과태료는 최대 3천만 원이고 계도기간은 1년(이상)이다 [다음](https://v.daum.net/v/20260121120209717), [ZDNet](https://zdnet.co.kr/view?no=20261020095628)
- 한국 성폭력처벌법은 딥페이크 소지·시청까지 처벌한다(최고 3년). 집중단속에서 1,438명을 검거했고 61.8%가 10대였다 [뉴시스](https://www.newsis.com/view/NISX20251114_0003403877)
- EU 50조: 2026-08-02부터 적용. 기존 시스템의 50조 2항 의무만 2026-12-02까지 유예됐고, 옴니버스 관보 게재는 미확인. 실천강령은 2026-06-10 확정 [William Fry](https://www.williamfry.com/knowledge/eu-ai-act-omnibus-deal-reached-postponed-deadlines-watermarking-compromise-and-the-nudificiation-prohibition/)
- 캘리포니아 SB 942/AB 853: 2026-08-02 시행, 위반 시 건당·일당 5,000달러. SB 1000은 2026-09-30 서명돼 즉시 시행(공식 leginfo 기록은 미확인) [MoFo](https://www.mofo.com/resources/insights/261001-california-revamps-ai-transparency-requirements)
- TAKE IT DOWN: 2026-05-19부터 FTC 집행. 48시간 안에 삭제해야 하고 위반 시 건당 최대 53,088달러. 2026-05-20 약 12개 사이트에 경고장을 보냈다 [FTC](https://www.ftc.gov/news-events/news/press-releases/2026/05/ftc-sends-warning-letters-companies-about-compliance-take-it-down-act)
- 중국 표시 규정(2025-09-01 시행): 2026-02 13,421개 계정 처벌(팩트체크 미확인) [TechNode](https://technode.com/2026/02/13/china-cyberspace-regulators-crack-down-on-unlabeled-ai-generated-content-penalize-over-13000-accounts/)
- Anthropic이 Claude 텍스트 워터마크 탐지 API를 발표했다는 보도가 있다. 날짜와 세부는 미확인 [The Decoder](https://the-decoder.com/anthropic-announces-watermark-detection-api-that-will-let-third-parties-detect-claudes-ai-texts/)

## 8. 검증에서 정정·삭제된 주요 사항

- **"SynthID 탐지는 비공개라 파트너십 없이는 통합할 수 없다"를 정정:** Google은 2026-05부터 기업용 AI Content Detection API를 제한 프리뷰로 제공하고 있다. 통합 경로가 열릴 수 있다는 뜻이면서, Google이 B2B 시장의 직접 경쟁자라는 뜻이다.
- **캘리포니아 SB 1000의 '출처 엇갈림'은 해소됨:** 2026-09-30 서명됐다(로펌 2곳 확인). 원 조사의 "명시 표시 옵션 의무"와 "생성기별 확인이 무료 상품이 된다"는 서술을 고쳤다. 제3자 검증도구로 의무를 이행할 수 있다는 기회 요인을 추가했다.
- **OpenAI Verify:** Research preview로 고쳤다. 'Content Provenance API'가 검증용 API인지는 불분명하다. 오디오 적용 범위는 출처마다 엇갈린다.
- **Sora 종료를 추가:** 원 조사는 Sora를 현역 서비스처럼 예로 들었다. WaPo C2PA 테스트는 2025-10 시점이라고 밝혔다.
- **C2PA 로열티를 '확인 못 함'에서 '로열티 프리'로 정정:** 비용은 CA 인증서 수수료뿐이다.
- **EU:** 옴니버스 관보 게재가 미확인이라는 점과 상호운용성 기한(2027-02-02)을 추가했다.
- **arXiv 2605.09203과 2607.16010:** 모두 재현되지 않은 프리프린트로 표시하고 confidence를 낮췄다. 텍스트 결과를 이미지·오디오로 일반화하지 않도록 했다.
- **경찰청 자체 탐지 SW를 추가:** B2G 진입 장벽으로 반영했다.
- **점수 조정:** OpenAI Verify 신뢰도를 3에서 2로 낮췄다. SynthID Detector 실사용 3은 '추정'으로 표시했다. Apple Reference Image 실사용을 3에서 2로 낮췄다(옵트인 모드, Pro 기종 한정).
- **반박되어 삭제된 주장:** 없음.
