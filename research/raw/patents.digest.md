# 특허·라이선스 장벽: 검증 반영 요약본 (2026-11-14 기준)

> 조사 결과(patents.research.json)와 2차 적대적 검증(실제 WebSearch 15회 사용)을 합친 요약본이다. 1차 검증(patents.verify.json)은 검색 없이 끝났으므로 반영하지 않았다. patents.google.com은 세션 네트워크 정책으로 막혀 있어 **청구항 전문은 원문으로 확인하지 못했다**. 서지 사항(번호, 등록일, 권리자)은 USPTO 공보와 Justia로 확인했다. 작성자는 변호사·변리사가 아니며, 이 문서는 FTO 검토를 대체하지 않는다.

## 1. 영역 요약
- 딥페이크 탐지·방지 특허 출원은 2018년 이후 급증했다. 출원 건수 1위는 **중국 CNIPA(1,288건)**로 압도적이고, 미국 205건, 한국 151건이 뒤를 잇는다([특허뉴스](http://e-patentnews.com/14873)).
- 확인한 등록 특허는 모두 특정 구현(PPG, 점수 결합, 교차모달 구조, 대상자별 모델 등) 단위다. "업로드하면 AI 생성 여부를 판별한다"는 개념 전체를 막는 포괄 특허는 발견되지 않았다. 다만 2025~2026년에는 저화질 탐지, 생성 도구 귀속, 음성 탐지처럼 범용 기능 영역에도 등록이 쌓이고 있다.
- 실제 소송은 탐지 모델이 아니라 프로비넌스(KeeeX v. C2PA, 2026-10 UPC 본안 심리 시작)와 라이브니스·eKYC(FaceTec v. iProov/Jumio, Prove v. KYXStart) 쪽에서 일어나고 있다.
- 가장 현실적인 장벽은 학습 데이터 라이선스다. 대표 벤치마크가 비상업 전용이다.
- 판정: 특허만 보면 진입은 가능하다. 다만 구현마다 회피 설계와 FTO가 필요하고, eKYC·C2PA로 확장하면 리스크가 높다.

## 2. 주요 권리·자원 표 (중요도 순)
이 영역은 앱이 아니라 특허·데이터 자원을 분석했다. 열은 이렇게 읽는다. 메이저성은 권리자의 영향력, 실사용은 상용 적용 여부, 신뢰도는 정보 확인 수준(1~5)이다.

| 권리/자원 | 회사(국가) | 형태 | 대상 | 메이저성 | 실사용 | 신뢰도 | 상태 | 근거 한 줄 |
|---|---|---|---|---|---|---|---|---|
| EP 2 949 070 (KeeeX v. OpenAI·Adobe·Truepic·C2PA) | KeeeX(프랑스) | 특허+UPC 소송 | 프로비넌스(C2PA) | 높음 | C2PA 구현 전반 | 4 | 2026-10 파리 본안 진행, 무효 반소, 판결 전 | [JUVE Patent](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/) |
| FaceTec 라이브니스 특허(50건) | FaceTec(미국) | 특허+소송 | 얼굴 라이브니스 | 높음 | eKYC 업계 | 4 | 2026-06 PTAB가 Jumio IPR 4건 기각해 특허 유지, iProov 소송 진행 중 | [Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents) |
| Pindrop US12142083B2 | Pindrop(미국) | 등록 특허 | 음성+영상 | 높음 | 콜센터 제품 | 4 | 2024-11-12 등록, 유효 | 화자·얼굴 딥페이크+인식+립싱크 점수 결합 [Justia](https://patents.justia.com/patent/12142083) |
| Reality Defender US12412376·US12411910·US12462813 | Reality Defender(미국) | 등록 특허 | 영상/음성 | 높음 | 자사 제품 | 3 | 2025-09-09 등록 2건, 2025-11-04 추가 등록 | 가짜 영상 ML 탐지, 오디오 가짜 탐지. 교차모달 구조는 미확인 [USPTO 공보](https://patentsgazette.uspto.gov/week44/OG/html/1540-1/US12462813-20251104.html) |
| Intel US12475695B2 | Intel(미국) | 등록 특허 | 얼굴·음성·텍스트 | 높음 | 미상 | 4 | 2025-11-18 등록 | 대상자별 로컬 학습 모델로 특정 인물 사칭 탐지 [USPTO 공보](https://patentsgazette.uspto.gov/week46/OG/html/1540-3/US12475695-20251118.html) |
| Intel US12125256B2 | Intel(미국) | 등록 특허 | 영상 | 중 | 미상 | 2 | 세부 사항 미확인 | 생성기 수정 기반 탐지(조사 원문 기준) [Justia](https://patents.justia.com/patent/12125256) |
| SUNY FakeCatcher US11687778B2·US12106216B2 | Research Foundation of SUNY(미국) | 등록 특허 | 영상(PPG) | 중 | Intel FakeCatcher 연관 | 2 | **미확인** | PPG 맵+CNN [Google Patents](https://patents.google.com/patent/US11687778) |
| US12586395·US12586419·US12548588 | 미상(미국 공개) | 등록/공개 | 영상·음성 | 중 | 미상 | 3 | 2025~2026 | 도구 귀속 탐지 모델, 저화질 탐지, 이중 트랙 가짜 음성 탐지 [USPTO PDF](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586395) |
| Originality.ai US12253988 | Originality.ai(캐나다) | 등록 특허 | 텍스트 | 중 | 자사 제품 | 4 | 2025-03-18 등록 | AI 탐지를 독립 청구한 것이 아니라 통합 텍스트 검증의 일부 [Justia](https://patents.justia.com/assignee/originality-ai-inc) |
| 누리랩 딥페이크 탐지 특허 | 누리랩(한국) | 국내 등록 | 영상/이미지 | 중(국내) | 자사 제품 | 3 | 2025-11 등록, 번호 미확인 | AI+메타데이터 이상 패턴 [보안뉴스](https://m.boannews.com/html/detail.html?idx=140194) |
| GenImage 데이터셋 | 학계(중국) | 데이터셋 | 이미지 | 높음 | 벤치마크 | 5 | CC BY-NC-SA 4.0+추가 약관, 상업 금지 | [GenImage](https://genimage-dataset.github.io) |
| FaceForensics++ | TUM(독일) | 데이터셋 | 영상 | 높음 | 벤치마크 | 3 | 비상업 연구·교육 전용(원 조사 기준) | [TUM ToS](https://kaldir.vc.in.tum.de/faceforensics_tos.pdf) |
| ASVspoof 2019/5 | 학계 컨소시엄 | 데이터셋 | 음성 | 높음 | 벤치마크 | 4 | ODC-By 1.0, 상업 허용 | [ASVspoof 2019 논문](https://arxiv.org/pdf/1911.01601) |
| TrueMedia.org 공개 코드 | TrueMedia(미국) | 오픈소스 | 다중 모달 | 중 | 서비스 종료 | 4 | MIT, 가중치 공개 보류, GenConViT는 GPL-3.0 | [TrueMedia 공지](https://www.truemedia.org/post/open-source-release) |
| Stanford GPIC | Stanford(미국) | 데이터셋 | 실사진 1억 장 | 중 | 신규 | 3 | 2026, 상업 이용 가능 | [arXiv](https://arxiv.org/pdf/2605.30341) |

## 3. 4개 기준 판정
점수 1~5. 이 영역에서는 높을수록 사용자에게 유리하다(장벽이 낮다는 뜻).

- **메이저성 (특허 장벽의 크기): 3/5.** 출원은 많다. IP5 기준 2024년 단년도 329건이고, 국가별 누적은 중국 1,288, 미국 205, 한국 151, 유럽 42, 일본 34건이다([특허뉴스](http://e-patentnews.com/14873)). 그러나 포괄 특허는 없다. 영향력이 큰 권리자는 Pindrop, Reality Defender, Intel, FaceTec이다. 조사 원안의 3.5에서 소폭 내렸는데, 중국 출원과 2025~2026년 신규 등록을 반영했다.
- **완성도·실사용 (권리 집행 실태): 3/5.** 탐지 특허 침해 소송은 extended 검색에서도 찾지 못했다(PACER 미조회). 반면 프로비넌스(KeeeX)와 라이브니스(FaceTec 등)는 실제로 소송이 진행 중이다.
- **신뢰도 (이 조사의 신뢰도): 3.5/5.** 핵심 서지 정보, KeeeX 항소심, Recentive 판례, GenImage·TrueMedia 라이선스는 독립 출처로 확인했다. 미확인 항목은 청구항 원문, SUNY 특허, Intel US12125256 세부 사항, C2PA 특허정책이다.
- **신규 진입 경쟁력 (특허 측면): 3/5.** 진입은 가능하다. 다만 범용 기능 영역에도 청구항이 생기고 있어 회피 설계 비용이 늘고 있다. 원안의 3.5에서 내렸다. eKYC나 C2PA 서명 기능을 붙이면 2/5 수준으로 떨어진다.

## 4. 레드오션 판정 (특허 측면): **부분적**
- 아니오 쪽 근거: 개념 전체를 막는 포괄 특허가 없다. 이 개념은 2019년 이전부터 논문(FaceForensics++, FakeCatcher)으로 공개돼 있다. 미국에서는 기존 ML을 새 데이터에 적용한 수준의 청구항은 §101로 무효가 될 수 있다([GT Law: Recentive v. Fox](https://www.gtlaw.com/en/insights/2025/4/federal-circuit-machine-learning-patents-ineligible-in-recentive-analytics-inc-v-fox-corp), 134 F.4th 1205, 2025-04).
- 예 쪽 근거: 같은 판결이 "ML 모델 자체의 개선"은 적격일 수 있다고 열어 두었다([Nixon Peabody](https://nixonpeabody.com/insights/alerts/2025/06/24/federal-circuit-limits-patent-eligibility-of-machine-learning-in-recentive-analytics-v-fox)). 따라서 아키텍처나 학습법을 청구한 Reality Defender·Pindrop류 특허는 이 판례로 쉽게 무효가 되지 않는다. 2025~2026년에는 저화질 탐지, 도구 귀속, 음성 탐지 특허가 늘고 있다([USPTO 12586419](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12586419), [USPTO 12548588](https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/12548588)). 중국 출원이 압도적이다.
- 결론: "특허로 막혀 포기"할 영역은 아니다. 다만 "구현 단위라 회피가 쉽다"는 낙관은 줄여야 하고, 인접 영역(eKYC·C2PA)은 실제 분쟁 지대다.

## 5. 빈틈·기회
- 음악 AI 생성 판별, 혼합 모달 통합 판별, 수사용 감정서(설명가능성)·증거보관연속성(chain-of-custody) 워크플로는 특허 밀도가 낮아 보인다(추론, 정량 근거 미확인).
- 확인된 특허는 구현 단위다. PPG 맵+CNN, 생체 임베딩+립싱크+딥페이크 점수 결합, 대상자별 로컬 모델 같은 조합을 피해 다른 특징·앙상블 구조를 쓰면 회피할 수 있다(추론).
- 자체 구현(수사용 증거 패키징, 모달 간 교차검증 방식)을 국내에 방어적으로 출원해 두면 투자 유치와 분쟁 협상에 쓸 수 있다(추론).
- 상업적으로 쓸 수 있는 데이터가 있다. ASVspoof 2019/5(ODC-By)([논문](https://arxiv.org/pdf/1911.01601)), Stanford GPIC 실사진 1억 장([AI Weekly](https://aiweekly.co/alerts/stanfords-gpic-ships-100m-commercially-usable-training-images))이 대표적이다. 여기에 최신 생성기로 직접 합성한 데이터를 더하면 비상업 벤치마크 의존을 피할 수 있다.
- TrueMedia 코드(MIT)는 참고용으로 쓸 수 있다([TrueMedia](https://www.truemedia.org/post/open-source-release)).

## 6. 위협·장벽
- **학습 데이터 라이선스(최대 장벽):** GenImage는 데이터셋과 파생물의 상업적 이용을 금지한다([GenImage](https://genimage-dataset.github.io)). FaceForensics++는 비상업 전용이다([TUM ToS](https://kaldir.vc.in.tum.de/faceforensics_tos.pdf), 독립 재확인은 못함). DeepfakeBench는 CC BY-NC 4.0이다([GitHub](https://github.com/sclbd/deepfakebench)). DFDC와 Celeb-DF의 약관 원문은 미확인이다.
- **프로비넌스(C2PA):** KeeeX 사건은 본안 심리 중이다. 2026-03-13 항소법원이 스위스·스페인·영국·아일랜드·노르웨이·폴란드 부분은 관할이 없다고 판단해 범위를 좁혔다([UPC 결정](https://www.unifiedpatentcourt.org/sites/default/files/files/api_order/922-2026%20Adobe%20ea%20Final%20Order%20en-GB.pdf), [Lavoix](https://www.lavoix.eu/the-upc-court-of-appeals-overturns-extraterritorial-jurisdiction-in-the-lawsuit-against-openai-and-adobe/?lang=en)). 2026-10 파리 지방부에서 본안 심리가 시작됐고, 피고 측은 무효 반소를 냈다([JUVE](https://www.juve-patent.com/cases/all-eyes-on-paris-as-keeex-case-on-the-merits-against-adobe-and-openai-kicks-off/)). C2PA 특허정책(로열티 프리 여부)은 미확인이다. KeeeX는 C2PA 비회원이므로, 정책이 로열티 프리라도 이 리스크는 남는다(추론).
- **라이브니스·eKYC:** FaceTec은 등록 특허 50건을 보유하고 있다([IDTechWire](https://idtechwire.com/facetec-reaches-50-issued-patents-with-uspto-grant-on-autonomous-authentication-nodes/)). 2026-06 PTAB가 Jumio의 IPR 4건을 기각했다([Biometric Update](https://www.biometricupdate.com/202606/appeals-board-upholds-4-facetec-biometric-liveness-detection-patents)). FaceTec v. Jumio(N.D. Cal. 3:24-cv-03623)([GreyB](https://ipverse.greyb.com/litigation/cases/case-details/facetec-inc-v-jumio-corporation--3-24-cv-03623))와 iProov 소송은 진행 중이다. 2026-10에는 Prove v. KYXStart 소송이 제기됐다([Biometric Update](https://www.biometricupdate.com/202610/prove-sues-kyxstart-over-patent-infringement-alleged-contract-interference)).
- **논문 방법을 그대로 제품화할 때의 리스크:** FakeCatcher식 PPG(SUNY 특허는 미확인), AV 교차검증(Pindrop 립싱크 점수 청구 포함)이 해당한다.
- **중국:** 출원 1,288건이고, 주요 출원인은 핑안·바이두·텐센트다([특허뉴스](http://e-patentnews.com/14873)). 중국에 진출하거나 중국 기술을 채택하면 FTO 범위를 넓혀야 한다.
- **GPL-3.0 구성요소(TrueMedia GenConViT):** 배포 형태에 따라 소스 공개 의무가 생길 수 있다([GitHub](https://github.com/truemediaorg/GenConViT)).
- **개인정보·초상권:** 데이터셋의 얼굴·음성은 개인정보와 초상권 문제가 있다. 수사용으로 쓰면 데이터 출처의 적법성이 증거능력 다툼 대상이 될 수 있다(추론).
- **상표:** "AI Detector"처럼 기능을 설명하는 이름은 식별력이 부족하다. FakeCatcher, Reality Defender 같은 기존 브랜드와 충돌할 수 있다. 9류·42류로 선행 조사가 필요하다(일반 가이드, 미확인(사전 지식)).

## 7. 핵심 사실 목록
1. IP5 딥페이크 탐지·방지 출원은 2024년 단년도 329건이다. 국가별 누적은 중국 1,288(핑안·바이두·텐센트), 미국 205, 한국 151, 유럽 42, 일본 34건이다. 이 보도의 국내 최다 출원인은 삼성전자·성균관대다([특허뉴스](http://e-patentnews.com/14873)). 반면 KISTI 집계는 LG전자 129, 삼성전자 35다([KISTI ScienceON](https://scienceon.kisti.re.kr/aiq/issue/selectIssueReportView.do?searchIssueRptNo=171&searchDataSectionId=tab_keyword)). 검색식에 따라 결과가 크게 다르다.
2. 특허청의 2021년 공식 통계는 탐지가 아니라 '딥페이크 기반 데이터 생성·증강' 분야다(2015년 37건→2018년 1,124건)([정책브리핑](https://m.korea.kr/briefing/pressReleaseView.do?newsId=156485475&pWise=main&pWiseMain=C3)).
3. Patsnap 'AI 생성 미디어 탐지' 스냅샷은 70여 건이다. HiddenLayer 7, Dropbox 6, BoA 4, MS·IBM·Google·Netskope·QOMPLX 각 3건이다(벤더 집계). HiddenLayer 건은 GenAI 모델 보호 위주다([Patsnap](https://www.patsnap.com/resources/blog/rd-blog/ai-generated-media-detection-technology-2026-patsnap-eureka/)). 영상 위조 탐지 랜드스케이프는 138건이다(벤더 집계)([Patsnap](https://www.patsnap.com/resources/blog/rd-blog/deepfake-video-forgery-detection-patent-landscape-patent-landscape/)).
4. Pindrop US12142083B2: 우선권 2020-10-16(가출원 63/092,956), 출원 17/503,152, 공개 2022-04-21, 등록 2024-11-12. 화자·얼굴 딥페이크, 화자·얼굴 인식, 립싱크 엔진의 점수를 결합한다([Justia](https://patents.justia.com/patent/12142083), [USPTO 공보](https://patentsgazette.uspto.gov/week46/OG/html/1528-2/US12142083-20241112.html)).
5. Reality Defender: US12412376 '가짜 영상 ML 탐지'와 US12411910 '오디오 가짜 탐지'가 2025-09-09 등록됐고, US12462813 B1이 2025-11-04 등록됐다([USPTO 공보](https://patentsgazette.uspto.gov/week36/OG/html/1538-2/US12411910-20250909.html)). 보유 12건은 GreyB 집계(벤더)이며 이미 늘었을 가능성이 높다([GreyB](https://insights.greyb.com/reality-defender-patents/)).
6. Intel US12475695: 출원 2021-09-22, 등록 2025-11-18. 대상자별 로컬 학습 모델에 얼굴·음성·텍스트 특징을 결합한다([USPTO 공보](https://patentsgazette.uspto.gov/week46/OG/html/1540-3/US12475695-20251118.html)).
7. Originality.ai US12253988: 출원 2024-03-08, 등록 2025-03-18. 통합 텍스트 검증 시스템이다([Justia](https://patents.justia.com/assignee/originality-ai-inc)). 두 번째 특허 12,705,435는 벤더 주장이다([Originality.ai](https://originality.ai/blog/originality-ai-patent)).
8. 누리랩 '딥페이크 생성물 탐지 방법 및 이를 수행하는 장치': 2025-02 출원, 2025-11 등록 보도가 있다. 등록번호는 미확인이다([보안뉴스](https://m.boannews.com/html/detail.html?idx=140194)). 딥브레인AI는 2024년 출원이 보도됐다([디지털데일리](https://m.ddaily.co.kr/page/view/2024020512542985882)).
9. 탐지 특허 침해 소송은 확인되지 않았다(PACER 미조회).
10. TrueMedia: 2025-01-13 이후 서비스를 종료했고, 2025-01-27 코드를 MIT로 공개했다. 2025-02-03 기준 "가중치는 아직 누구에게도 공유되지 않음" 상태다([TrueMedia](https://www.truemedia.org/post/open-source-release), [GeekWire](https://www.geekwire.com/2025/truemedia-org-plans-to-shutter-and-open-source-its-ai-deepfake-detector-etzioni-hints-at-new-startup/)).
11. Google SynthID Text는 HF Transformers v4.46.0+에 오픈소스로 구현돼 있다. 특허 여부는 미확인이다([Google](https://ai.google.dev/responsible/docs/safeguards/synthid?hl=en)).
12. Microsoft·Adobe·Samsung·Sony·중국 빅테크의 탐지 전용 특허 번호는 미확인이다.

## 8. 검증에서 정정·삭제된 주요 사항
- **중국 수치 보완:** "중국 미확인"을 CNIPA 1,288건(1위)으로 바꿨다. 국가별 수치(누적)와 329건(2024 단년도)이 서로 다른 기준임을 명시했다.
- **KeeeX:** "본안 결론 미확인"을 "2026-10 파리 본안 심리 시작, 무효 반소, 판결 전"으로 업데이트했다.
- **라이브니스 리스크 상향:** FaceTec PTAB 승소(2026-06), Jumio 소송, 특허 50건, Prove v. KYXStart를 추가했다.
- **Recentive v. Fox:** 사전 지식에서 확인됨으로 바꿨다. 다만 "ML 모델 자체 개선은 적격 가능"이라는 단서를 추가해, 구현 특허 리스크가 줄어든다는 해석을 철회했다.
- **Pindrop:** 청구 구조에 립싱크 점수와 얼굴 인식·딥페이크 엔진을 추가했다. 우선일은 2020-10-16으로 정정했다.
- **Reality Defender:** "교차모달 구조" 청구항 내용을 미확인으로 바꿨다. US12462813 추가 등록을 반영했다.
- **Intel:** US12475695는 확인됐다. US12125256 세부 사항은 미확인이다. Daily Upside 기사는 두 특허가 아니라 합성 데이터 증강 출원에 관한 것이다.
- **SUNY FakeCatcher 특허:** 원 조사의 신뢰도 high를 미확인으로 하향했다.
- **TrueMedia 가중치:** "이메일 요청으로 획득 가능"을 "공개 보류, 제공 여부 불확실"로 정정했다.
- **Originality.ai:** 독립 출처(Justia)로 확인했다. AI 탐지를 독립 청구한 특허가 아님을 명시했다.
- **Patsnap 70여 건:** 시장 전체 규모로 해석하지 않도록 했다. 138건 영상 랜드스케이프를 추가했다.
- **신규 특허 추가:** US12586395, US12586419, US12548588을 추가했다. 이에 따라 회피 설계 낙관론과 점수를 하향했다.
- **신규 데이터 대안 추가:** Stanford GPIC를 추가했다.
- **미확인 유지:** C2PA 특허정책, FaceForensics++ 약관 독립 확인, SUNY 특허 번호.
- **삭제(refuted):** 없음.
