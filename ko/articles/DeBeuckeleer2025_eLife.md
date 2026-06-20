# Unbiased identification of cell identity in dense mixed neural cultures

## Citation (NLM)
De Beuckeleer S, Van De Looverbosch T, Van Den Daele J, Ponsaerts P, De Vos WH. Unbiased identification of cell identity in dense mixed neural cultures. eLife. 2025;13:RP95273. doi: 10.7554/eLife.95273

**DOI:** [https://doi.org/10.7554/eLife.95273](https://doi.org/10.7554/eLife.95273)

---

## Background
- iPSC 기술이 뇌 상주 세포 유형(뉴런, 성상교세포, 미세아교세포 등) 생성 가능하나, iPSC 라인 간 변이와 세포 유형 포괄적 특성분석 기술 부재가 전임상 스크리닝 적용 장애
- 밀집·혼합 신경 배양에서 세포 유형 조성 정량적·체계적 특성분석 필요
- 기존 세포 유형 식별은 population-level time in culture 기준 분류로 부정확
- 단일 세포 수준 형태학적 프로파일링으로 복합 혼합 신경 배양 세포 조성 정량화 가능

## Key Experiment Methods
1. **Cell painting 기반 이미징 어세이**: 다중 형광 염색으로 세포 형태학적 특징(핵, 세포질, 액틴, 미토콘드리아 등) 시각화, high-content microscopy로 이미지 획득
2. **CNN 기반 세포 유형 분류**: convolutional neural network으로 cell painting 이미지에서 세포 유형 인식, neuroblastoma·astrocytoma pure/mixed cultures로 벤치마크
3. **Regionally restricted cell profiling**: 핵 ROI(nuclear region of interest) + 주변 환경만으로 전체 세포 이미지와 동등한 분류 정확도 달성, 밀집 배양에서도 예측 정확도 유지
4. **Iterative data erosion**: 입력 이미지 영역 단계적 축소로 최소 필요 ROI 확인, 핵+주변 환경이 분류에 충분함 입증
5. **iPSC 유래 신경 배양 적용**: 분화 상태 평가(성숙 뉴런 vs 신경 전구세포 비율), microglia 뉴런과 명확히 구분(반응 상태 무관), tiered strategy로 활성화 vs 비활성화 상태 추가 분류
6. **최적화 파라미터**: ROI 정의(핵+주변 vs 전체 세포), CNN 아키텍처, classification 임계값, cell painting 염색 조합, 이미지 해상도

## Results
- Cell painting + CNN 분류 정확도 >96%(neuroblastoma/astrocytoma pure/mixed cultures)
- Regionally restricted profiling(nuclear ROI + 주변)이 전체 세포 이미지와 동등한 정확도, semi-confluent 및 very dense cultures에서도 유지
- iPSC 유래 신경 배양에서 세포 기반 예측이 population-level time 기준 분류 대비 우수(96% vs 86%)
- Mixed iPSC 유래 신경 배양에서 microglia가 뉴런과 명확히 구분, 반응 상태 무관
- Tiered strategy로 활성화 vs 비활성화 microglia 추가 분류 가능(정확도 낮으나 식별 가능)
- 형태학적 단일 세포 프로파일링이 복합 혼합 신경 배양 세포 조성 정량화에 유효함 입증

## Perspective
- Cell painting + CNN이 iPSC 유래 세포 배양 품질 관리의 빠르고 저렴한 어세이로 기여
- Regionally restricted profiling이 밀집 배양에서도 적용 가능, 실제 전임상 스크리닝 환경에 적합
- 단일 세포 수준 분석이 배치 간·라인 간 변이 모니터링에 기여
- 향후 다중 세포 유형 동시 분류, 질병 모델 검증, 약물 스크리닝 품질 관리로 확장
- 자동화 이미징과 결합하여 iPSC 기반 신경 질환 모델 고속 특성분석 가능

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
