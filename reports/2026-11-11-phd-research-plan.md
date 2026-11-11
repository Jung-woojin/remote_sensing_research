# 박사 지원용 연구계획서 탐색: 나에게 맞는 항공·위성 CV 연구는 무엇인가?

- 작성일: 2026-11-11 (Asia/Seoul)
- 목적: 커리큘럼 설계가 아니라, 현재 이력에서 가장 설득력 있는 박사 연구주제를 비교·선정하고 지원서의 연구계획서 초안으로 연결한다.
- 결론: **시점 차이를 인지하는 항공–위성 크로스뷰 정합과 신뢰도 기반 위치추정**을 1순위로 권고한다.
- 영문 작업명: **Change-Aware Cross-View Alignment for Reliable UAV-to-Map Localization**
- 범위를 “UAV-to-satellite retrieval” 하나로 한정하지 않는다. 항공 영상, 위성 지도, 서로 다른 촬영 시점 사이의 정합·변화·불확실성을 함께 다룬다.
- Sentinel-2 해재질 세그멘테이션, 저고도 항공 객체탐지, KHOA 해양 과제는 모두 조건이 달라진 지리공간 영상에서 의미 있는 정보를 꺼내는 경험으로 묶인다.
- 고해상도 위성, 다중시기 변화탐지, VLM/오픈보카의 공백은 주제를 포기할 근거가 아니라, 첫 제안에서 명시적으로 관리할 검증 위험이다.
- 교토대 Ken Sakurada 교수는 주제 언어상 가장 가까운 우선 접촉 후보이지만, 독립적인 박사 지도 단위인지와 실제 수용 가능성은 공개 페이지로 확정할 수 없다.
- 아래의 점수는 논문 성능 비교가 아니라 지원자-주제 적합도에 대한 판단이다.

---

## 1. 출발 이력: 이미 있는 자산과 실제 공백

### 이미 있는 자산

| 이력 | 연구계획서에서의 의미 |
| --- | --- |
| Sentinel-2 기반 해재질 세그멘테이션 (SCI Q2) | EO 데이터, 물리·환경 조건 변화, 픽셀 단위 인식의 경험 |
| 저고도 항공 객체탐지 (IEEE Access) | 항공 플랫폼의 시점·스케일·촬영 조건에 대한 경험 |
| KHOA 해양 과제 | 연안·해양 운영 문제를 연구 질문으로 바꾸는 응용 맥락 |
| 해무 CCTV 연구 흐름 | 가시성·기상 조건 변화가 시각 인식에 미치는 영향을 다룬 경험 |

### 공백과 해석

| 공백 | 해석 |
| --- | --- |
| VLM / open-vocabulary | 첫 지원 주제의 중심 방법으로 삼기에는 증거가 부족하다. 필요하면 변화 설명 또는 불확실성 보고의 보조 모듈로 제한하는 편이 안전하다. |
| 다중시기 변화탐지 | 추천 주제의 핵심 검증 위험이다. 따라서 “변화탐지 성능 경쟁”보다 **변화가 정합·위치신뢰도에 미치는 영향의 분리**로 질문을 좁힌다. |
| <1m 고해상도 위성 | UAV↔지도 정합에 필요하지만 Sentinel-2 경력의 단절을 뜻하지는 않는다. 해상도·센서·시점 차이를 다루는 전이 문제로 연결한다. |

**지원 서사:** “해양 EO → 저고도 항공 인식 → 서로 다른 플랫폼·시점의 지리공간 영상을 신뢰 가능하게 연결하는 CV”이다. 주제의 중심은 해양 자체가 아니라, 항공·위성 관측의 조건 변화 속에서 믿을 수 있는 공간 인지를 만드는 일이다.

---

## 2. 후보 방향 비교

점수는 5점 만점의 **지원 적합도 판단**이며, 객관적 분야 순위가 아니다.

| 후보 | 기존 이력 연결 | CV·항공 정체성 | 차별화 여지 | 랩 접점 | 박사 리스크 | 판단 |
| --- | ---: | ---: | ---: | ---: | ---: | --- |
| A. 해양·연안 EO + 오픈보카 변화탐지 | 5 | 2 | 3 | 4 | 3 | 안전하지만 항공 정체성이 약해질 수 있음 |
| B0. 일반 UAV↔위성 cross-view 위치추정 | 3 | 5 | 2 | 3 | 3 | 핵심 벤치마크·대형 데이터셋이 빠르게 경쟁 중 |
| **B1. 변화 인지형 항공–위성 정합·신뢰도 위치추정** | **4** | **5** | **4** | **4** | **3** | **권고** |
| C. VLM 기반 원격탐사 변화 설명 | 2 | 1 | 3 | 4 | 2 | 현재 이력과 방법 공백이 모두 큼 |

### 왜 A만으로는 부족한가

A는 Sentinel-2·해양 과제와 가장 자연스럽게 이어지고 원격탐사 랩에 폭넓게 지원할 수 있다. 하지만 항공 탐지 논문과 항공전자공학 정체성을 부차화한다. 또한 open-vocabulary 변화탐지는 데이터·언어 정렬·평가 정의가 모두 경쟁적인 영역이라, 기존 성과를 “해양 응용”으로만 해석하게 만들 위험이 있다.

### 왜 B0도 그대로는 부족한가

드론–위성 위치추정은 매력적이지만, 단순 retrieval/registration은 이미 데이터와 방법이 빠르게 쌓이는 중이다. University-1652는 1,652개 건물, 72개 대학으로 구성된 drone↔satellite 과제를 제공한다. UniGeoRS는 satellite–drone–ground tri-view 벤치마크를 제시했다. 따라서 “두 시점의 특징을 잘 맞추겠다”는 서술만으로는 박사 제안의 연구 공백이 되기 어렵다.

### 최종 선택 B1

B1은 A와 B의 교집합이다. 지도와 항공 영상 사이의 시간 차이를 변화탐지 문제로 보고, 정합 실패를 단순 오차가 아닌 **원인별 위험**으로 다룬다. 이 방식이면 항공·자율비행 문맥에서는 GPS-denied/지도 기반 위치추정으로, 원격탐사 문맥에서는 multi-temporal cross-sensor change-aware registration으로 설명할 수 있다.

---

## 3. 추천 연구 주제

## 시점 차이를 인지하는 항공–위성 크로스뷰 정합과 신뢰도 기반 위치추정

### 문제 정의

항공 영상과 위성 지도는 촬영 고도·각도·해상도·센서·계절·건설 변화가 서로 다르다. 정합 결과가 틀렸을 때 현재의 시스템은 대체로 “위치가 틀렸다”는 하나의 실패로만 취급한다. 그러나 실제로는 다음이 구분되어야 한다.

1. **위치 오류:** 비슷한 다른 장소에 잘못 정합되었다.
2. **지도 노후화/실제 변화:** 위치는 맞지만 도로·건물·항만 구조 등이 달라졌다.
3. **관측 조건 차이:** 시점, 계절, 조명, 시야각, 해상도 차이로 대응점이 사라졌다.
4. **복합 불확실성:** 어느 설명도 충분하지 않아 자동 위치 결정을 보류해야 한다.

### 연구 질문

- **RQ1.** 어떤 시각 단서가 시점·시야가 달라도 안정적인 항공–위성 대응점으로 남는가?
- **RQ2.** 정합 불일치에서 “wrong location”과 “correct location but stale/changed map”을 분리할 수 있는가?
- **RQ3.** 변화 증거를 조건으로 사용하면 위치추정의 calibration과 selective prediction(필요 시 보류)을 개선할 수 있는가?
- **RQ4.** 도시뿐 아니라 항만·연안처럼 구조물 변화와 관측 조건 변화가 큰 지역에도 전이되는가?

### 가설

> 변화에 둔감한 특징만으로 위치를 고르는 모델보다, **안정 구조의 기하 정합**과 **변화 가능 영역의 별도 추정**을 함께 수행하는 모델이 지도 노후화 상황에서 더 잘 보정된 위치 신뢰도를 낸다.

### 최소한의 방법 설계

거대한 VLM을 전제하지 않는다. 첫 논문은 검증 가능한 두 갈래 구조로 충분하다.

- **Stable-correspondence branch:** 도로 윤곽, 장기 구조물, 교차로 등 시점 변화에 비교적 안정적인 단서로 정합 후보를 점수화한다.
- **Change-evidence branch:** 후보 위치에서 사라지거나 새로 생긴 영역을 변화 증거로 산출한다.
- **Decision layer:** 위치 점수와 변화 증거를 이용해 위치, 지도 노후화 가능성, 또는 보류를 출력한다.

핵심 기여는 “더 높은 retrieval 점수” 하나가 아니라, **실패의 원인을 구분하고 그 불확실성을 정량화하는 공간 인지**다.

---

## 4. 최신 연구 지형과 차별화

### 사실: UAV↔satellite registration은 이미 실전 조건으로 확대 중

WACV 2026의 AirLock+는 UAV-to-satellite 정합을 목표 위치 지리추정으로 다루며, 심한 domain gap, 오래된 위성영상, 보지 못한 환경을 다룬다고 설명한다. 저자들은 고고도 사선 영상의 실제 궤적에서 평균 20.23m 목표 위치 오차를 보고했다. 이는 추천 주제의 필요성을 강하게 뒷받침하지만, 동시에 “outdated map에서도 registration” 자체는 새롭지 않다는 경고다.

**해석:** 이 제안은 AirLock+의 registration 성능 경쟁을 반복하지 않는다. 시간적 불일치가 관측되었을 때 위치 오류와 변화의 원인을 분리하고, 잘못된 자동 결정을 피하는 calibration으로 질문을 옮긴다.

### 사실: 단순 cross-view retrieval의 벤치마크화가 진행 중

CVPR 2026의 UniGeoRS는 satellite, drone, ground의 tri-view geo-localization을 위한 통합 벤치마크와 프레임워크를 제시한다. ICCV 2025의 MMGeo는 UAV 위치추정에 image, point cloud, depth, text를 결합하는 방향을 제안한다.

**해석:** 새 모달리티를 무작정 더하는 것은 충분한 차별화가 아니다. 지원자의 자연스러운 진입점은 “어떤 상황에서 위치 결과를 믿지 말아야 하는가”라는 신뢰도 문제다.

### 사실: 변화분석용 VLM 자원도 등장하고 있다

DeltaVLM은 remote-sensing change analysis를 위한 VLM 프레임워크와 ChangeChat-105k를 공개했다.

**해석:** VLM은 최종 연구의 설명·변화 가설 생성에 유용할 수 있다. 그러나 지원자에게는 먼저 기하·시점·지도 변화의 검증 가능한 문제를 세우고, VLM은 보조 도구로 두는 편이 연구계획서의 인과 구조가 더 강하다.

---

## 5. 데이터와 평가: 주장하지 말고 검증할 것

### 사용할 수 있는 출발점

- **University-1652:** drone-to-satellite 및 satellite-to-drone 과제를 제공하는 공개 기준선이다. 서로 다른 대학의 train/test 분할로 일반화 평가가 가능하다.
- **UniGeoRS / GeoBridge:** tri-view 및 대규모 cross-view 지리추정이 어떤 데이터·프로토콜로 흘러가는지 확인하는 비교 대상이다. GeoBridge는 공개 제약이 있는 소스 이미지도 있으므로 실제 재현 가능 범위를 먼저 확인해야 한다.
- **공개 고해상도 항공·지도 자료:** 면허와 촬영 시점이 명확한 자료만 실제 temporal-change 평가에 포함한다. 접근 불가한 상용 타일을 재배포하거나 출처가 불명확한 조합을 데이터셋으로 주장하지 않는다.

### 평가 프로토콜

주장보다 먼저 네 가지 실패 셀을 명시한다.

| 실제 위치 | 지도 시점 | 기대 행동 |
| --- | --- | --- |
| 정확 | 일치 | 정확한 위치와 높은 신뢰도 |
| 정확 | 불일치 | 위치 유지 또는 변화 증거 제시 |
| 오답 | 일치 | 오답 위치 거부 |
| 오답 | 불일치 | 보류 또는 낮은 신뢰도 |

보고할 측정치는 retrieval Recall@K, 거리/registration error, 변화·노후 지도 탐지 AUROC, calibration error(ECE), risk–coverage curve다. 이 조합은 위치정확도만 높이고 위험한 확신을 내는 방법을 걸러낸다.

---

## 6. 지원서에 쓸 수 있는 1문단 연구계획서 초안

> My doctoral research will study reliable geospatial perception across aerial and satellite imagery acquired from different viewpoints and times. Existing UAV-to-map localization often treats mismatch as a single localization error, even though it can arise from map staleness, physical scene change, or viewpoint-induced appearance shift. I propose to separate stable geometric correspondence from change evidence and to use both for calibrated localization and selective abstention. Building on my experience in Sentinel-2 marine-material segmentation and low-altitude aerial object detection, I will evaluate whether temporal-change-aware alignment improves localization reliability across urban and coastal environments. The goal is not only to localize an aerial observation, but to state when its map-based location should or should not be trusted.

---

## 7. 랩·지원 전략

### 1순위 확인 대상: Kyoto University, Ken Sakurada

교토대 공식 프로필은 Sakurada 교수를 Graduate School of Informatics, Department of Informatics의 Associate Professor로 기재하며, 연구 관심사에 3D modelling, change detection, sensor-data privacy와 computer vision, robotics, remote sensing을 포함한다. 교토대 공학 연구실 안내에는 “Spatial Context Sensing Research Project”로 표시된다.

**확인된 사실과 미확인 사항을 분리한다.**

- 확인: 교토대 정보학연구과의 현직 소속과 변화탐지·3D 모델링·원격탐사 접점.
- 미확인: 독립 랩 운영 여부, 박사 단독 지도 권한·정원, 2027년 실제 수용 의사, 니시노 그룹과의 행정적 지도 구조.
- 따라서 첫 연락의 질문은 “제 주제에 관심이 있는가”만이 아니라, **박사 과정에서의 주지도 체계와 입학 전 승인 절차**여야 한다.

### 입시 사실

교토대 정보학연구과 영문 입시 안내는 해외 대학 졸업자에게 AAO 사전심사, 지원 전 희망 지도교수 또는 준교수의 승인 절차가 필요할 수 있음을 안내한다. 2027년 4월 박사과정 일정은 과정별로 달라질 수 있으며, 공개된 일정표 자체도 변경 가능성을 고지한다. 따라서 일정은 공식 페이지를 기준으로 보고, 지원 과정과 지도 가능 여부를 교수에게 확인해야 한다.

### 접촉 메일에서 보여줄 자료

커리큘럼이 아니라 아래 세 장이면 충분하다.

1. 위 1문단 연구계획서와 연구 질문 3개.
2. 기존 Sentinel-2·항공 탐지 논문을 한 장에 연결한 “prior evidence” 도식.
3. 위치 오류와 지도 변화의 네 실패 셀을 보여주는 작은 예비 분석 그림.

---

## 8. 결론과 보류해야 할 선택

- **선택:** B1, 변화 인지형 항공–위성 정합과 신뢰도 위치추정.
- **A를 버리지 않는 방식:** 연안·항만을 전이 검증 영역으로 사용한다. 해양 EO 경험은 응용의 중심이 아니라 일반화가 어려운 조건의 설득력 있는 사례가 된다.
- **B0를 피하는 방식:** “더 잘 찾는 retrieval”만 주장하지 않고, 틀릴 때 왜 틀렸는지와 언제 보류할지를 연구한다.
- **VLM을 과장하지 않는 방식:** 첫 제안의 핵심 가설 검증 이후 변화 설명 보조수단으로만 확장한다.
- **항만 CCTV 시정 논문:** 독립된 가시성 논문으로 두면 서사가 분산될 수 있다. 다음 결과물이 이 주제를 강화하는지(조건 변화·교차 플랫폼·안전한 의사결정) 기준으로 우선순위를 재평가한다.

---

## Sources

1. AirLock+ (WACV 2026): https://openaccess.thecvf.com/content/WACV2026/html/Deng_AirLock_Scaling_UAV-to-Satellite_Image_Registration_for_Target_Geolocalization_and_Geospatial_WACV_2026_paper.html
2. UniGeoRS (CVPR 2026): https://openaccess.thecvf.com/content/CVPR2026/html/Liang_UniGeoRS_A_Unified_Benchmark_for_Tri-view_Geo-Localization_CVPR_2026_paper.html
3. MMGeo (ICCV 2025): https://openaccess.thecvf.com/content/ICCV2025/html/Ji_MMGeo_Multimodal_Compositional_Geo-Localization_for_UAVs_ICCV_2025_paper.html
4. University-1652 baseline: https://github.com/layumi/University1652-Baseline
5. GeoBridge: https://github.com/MiliLab/GeoBridge
6. DeltaVLM: https://github.com/hanlinwu/DeltaVLM
7. Kyoto University — Ken Sakurada profile: https://kdb.iimc.kyoto-u.ac.jp/profile/en.08e1c834541f610e.html
8. Kyoto University — Visual Information Processing Laboratory: https://www.s-ee.t.kyoto-u.ac.jp/ja/information/laboratory/vip
9. Kyoto University Graduate School of Informatics, application: https://www.i.kyoto-u.ac.jp/en/admission/application/
10. Kyoto University doctoral schedule: https://www.i.kyoto-u.ac.jp/en/admission/guide/schedule_doctor/
