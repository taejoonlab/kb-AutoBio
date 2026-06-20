# An autonomous laboratory for the accelerated synthesis of novel materials

## Citation (NLM)
Szymanski NJ, Rendy B, Fei Y, Kumar RE, He T, Milsted D, McDermott MJ, Gallant M, Cubuk ED, Merchant A, Kim H, Jain A, Bartel CJ, Persson K, Zeng Y, Ceder G. An autonomous laboratory for the accelerated synthesis of novel materials. Nature. 2023;624:86-93. doi: 10.1038/s41586-023-06734-w

**DOI:** [https://doi.org/10.1038/s41586-023-06734-w](https://doi.org/10.1038/s41586-023-06734-w)

---

## Background
- 계산 재료과학의 발전으로 대규모 ab initio 스크리닝을 통한 신물질 발견이 가능해졌으나, 실험적 검증은 여전히 느리고 노동집약적임
- 자율성(autonomy)을 갖춘 실험 플랫폼이 필요: 데이터를 해석하고基于해 의사결정을 할 수 있는 실험 에이전트
- 기존 자율 실험실 연구는 탄소나노튜브 수율, 광전 성능, 광촉매 활성 등 특정 분야에 제한적이었음
- 고체 무기 분말 합성은 액체 처리와 달리 분쇄, 밀링 등 고유한 도전과제가 존재

## Key Experiment Methods
1. **A-Lab 플랫폼 구성**: 시료 준비(분말 계량·혼합), 가열(4개 box furnace), 특성분석(XRD)의 3개 스테이션을 로봇 암으로 연결, API 기반 온디맨드 작업 제출
2. **합성 레시피 생성**: 문헌에서 text-mining한 합성 데이터로 학습한 ML 모델이 유사 물질 기반 초기 레시피 제안(전구체 조합), 제2의 ML 모델이 합성 온도 제안
3. **ARROWS3 능동학습 알고리즘**: 합성 실패 시 pairwise reaction 분석(88개 고유 반응 DB 구축), 동일 중간생성물 경로 80%까지 탐색 공간 축소, Materials Project formation energy로 큰 driving force를 가진 중간생성물 우선 선택
4. **XRD 패턴 분석**: ICSD 기반 확률적 ML 모델로 상 동정, 자동 Rietveld 정밀화로 확인, 목표 상 수율(>50%) 평가
5. **타겟 선정**: Materials Project와 Google DeepMind의 phase-stability 데이터에서 convex hull 상 또는 근처(<10 meV/atom)에 있는 58개 신규 화합물 선정, 공기 중 안정성 필터링(O2, CO2, H2O와 반응하지 않는 것만)

## Results
- 17일 연속 폐쇄루프 운영, 총 355개 실험 수행, 58개 타겟 중 41개 합성 성공 (성공률 71%, >2개 신규 물질/일)
- 355개 레시피 중 130개(37%)만 목표 생성 → 전구체 선택이 합성 경로 결정에 핵심 영향
- 문헌 기반 ML 레시피로 35개 합성 성공(초기 레시피), 능동학습으로 9개 타겟 수율 개선(이 중 6개는 초기 수율 0%)
- 능동학습 최적화 사례: CaFe2P2O9 합성에서 FePO4+Ca3(PO4)2 경로(driving force 8 meV/atom) 회피, CaFe3P3O13 중간생성물 경로(77 meV/atom) 선택으로 수율 ~70% 증가
- 17개 실패 원인 분류: 반응 속도 지연 11개(<50 meV/atom driving force), 전구체 휘발(CaCr2P2O9, ammonium phosphate 450°C 이상 증발), 비정질화(Mo(PO3)5, phosphate-rich glass 형성), 계산 부정확(La5Mn5O16, YbMoO4, BaGdCrFeO6 - DFT pseudopotential/Jahn-Teller/f-state 문제)
- 수동 재분쇄+고온 가열로 Y3Ga3In2O12, Mg3NiO4 추가 합성 성공 → 성공률 74%로 향상, 계산 오류 화합물 제외 시 78%(43/55) 가능
- 분해 에너지와 합성 성공 간 명확한 상관관계 없음, 메타안정 화합물도 합성 가능

## Perspective
- AI 기반 자율 실험실이 계산 예측과 실험 검증 간 격차를 해소할 수 있음을 입증
- ab initio 계산, ML 알고리즘, 문헌 지식, 로봇공학의 통합이 재료 발견 가속화의 핵심
- 실패 사례 분석은 계산 재료 스크리닝의 한계(metastability 예측, 반응 동역학 등)를 보여주고 개선 방향 제시
- 향후 액체 처리, 박막 합성, 전기화학 평가 등 다른 합성 영역으로 확장 가능
- 인간 연구자와 자율 시스템의 협업 패러다임 정립 필요

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
