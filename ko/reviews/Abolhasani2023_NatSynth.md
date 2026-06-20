# The rise of self-driving labs in chemical and materials sciences

## Citation (NLM)
Abolhasani M, Kumacheva E. The rise of self-driving labs in chemical and materials sciences. Nat Synth. 2023;2(6):483-492. doi: 10.1038/s44160-022-00231-0

**DOI:** [https://doi.org/10.1038/s44160-022-00231-0](https://doi.org/10.1038/s44160-022-00231-0)

---

## Overview

화학·소재 분야에서 **Self-Driving Labs (SDLs)**의 개념, 현황, 구현 로드맵을 소개하는 리뷰. SDL은 머신러닝(ML) 알고리즘이 다음 실험 조건을 선택하고, 로봇이 시약 준비→합성→정제→분석의 폐쇄 루프(closed-loop)를 자동 수행하는 지능형 실험 플랫폼이다. 기존 화학·소재 연구의 핵심 병목—실험 단계 간 물리적 단절, 실험 후 의사결정까지의 시간 지연, 변수 탐색의 비효율—을 동시에 해결하는 방향을 제시한다.

---

## Key Topics

**SDL의 정의와 구성 요소**
- 하드웨어 모듈: 시약 준비, 합성(flow reactor/batch reactor/기판), 정제, 처리(processing), 분석(UV-Vis, NMR, HPLC 등)
- 소프트웨어 모듈: ML 모델(Gaussian Process 등), 불확실성 정량화, 유전 알고리즘 기반 실험 선택
- 샘플 이동 방식: 고정 로봇 암, 이동 로봇 암, 펌프/튜브/밸브

**SDL 구현 사례 (화학·소재 분야)**
- 반도체·금속 나노입자: 기존 대비 1,000배 빠른 합성-물성 매핑
- 페로브스카이트 양자점: 250회 자율 실험으로 키랄성 나노입자 발굴
- 박막 소재: 이전 기술 대비 50°C 낮은 저온 공정 조건 발굴
- 광촉매: 8일 연속 무감독 운전(688회 실험)으로 수소 발생 효율 6배 향상
- 의약품 원료물질(API): 온디맨드 현장 합성
- 3D 프린팅 구조체: 격자 탐색 대비 60배 적은 실험으로 최고 인성(toughness) 구조 발굴

**비전문가를 위한 SDL 로드맵**
- 하드웨어 선택: 목표 분자/소재 → 반응 상태(기체/액체/고체) → 필요 분석 기술 순으로 모듈 결정
- 소프트웨어 선택: 탐색 목표(발견/최적화/메커니즘 규명)에 따라 ML 알고리즘 결정
- 표준화된 데이터 표현 및 메타데이터 추적: 실험실 간 재현성 확보의 핵심

**현재 한계**
1. 표준화되고 비용 효율적인 하드웨어 부재
2. 접근성 높은 소프트웨어 부재
3. 화학자·소재 과학자를 위한 사용자 친화적 지침 부재
4. 물리 기반 모델(physics-based model)과 자율 실험의 통합 부재

---

## Key Findings

- SDL은 기존 변수 1개씩 탐색 방식 또는 조합 탐색 대비 **10~1,000배**의 연구 가속도를 달성
- SDL이 연구자를 대체하는 것이 아니라, 반복적 실험을 자동화하여 연구자가 고차원적 과학 문제에 집중할 수 있도록 보조
- 최소 투자로 시작하려면: 기존 분석 장비를 ML 소프트웨어와 연결하는 반자동(semi-autonomous) SDL이 현실적 첫 단계
- SDL의 closed-loop 데이터는 복잡한 다단계 반응의 메커니즘 규명에도 활용 가능
- 코로나19 팬데믹이 "현장 의존적" 연구의 취약성을 드러내며 SDL 필요성을 부각

---

## Perspective

SDL은 에너지, 지속 가능성, 헬스케어 분야의 글로벌 문제 해결을 가속화할 핵심 기술로 평가된다. 특히 복잡한 다단계 반응과 고차원 설계 공간이 필요한 분야에서 기존 연구 속도를 획기적으로 높일 잠재력이 있다. 향후 과제는 표준화된 SDL 하드웨어·소프트웨어 생태계 구축, physics-informed ML 통합, 그리고 에너지 소재·소분자 분야를 넘어 생물학적 복합 분자 합성으로의 확장이다.

---

## Key References

- Shields BJ et al. (2021) Bayesian reaction optimization as a tool for chemical synthesis. *Nature* 590:89-96. [doi:10.1038/s41586-021-03213-y](https://doi.org/10.1038/s41586-021-03213-y)
- Burger B et al. (2020) A mobile robotic chemist. *Nature* 583:237-241. [doi:10.1038/s41586-020-2442-2](https://doi.org/10.1038/s41586-020-2442-2)
- Coley CW et al. (2020) A robotic platform for flow synthesis of organic compounds informed by AI planning. *Science* 365:eaax1566. [doi:10.1126/science.aax1566](https://doi.org/10.1126/science.aax1566)
- Martin HG et al. (2023) Perspectives for self-driving labs in synthetic biology. *Curr Opin Biotechnol* 79:102881. [doi:10.1016/j.copbio.2022.102881](https://doi.org/10.1016/j.copbio.2022.102881)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
