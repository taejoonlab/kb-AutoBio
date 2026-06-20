# Sparks of function by de novo protein design

## Citation (NLM)
Chu AE, Lu T, Huang PS. Sparks of function by de novo protein design. Nat Biotechnol. 2024;42(2):203-215. doi: 10.1038/s41587-024-02133-2

**DOI:** [https://doi.org/10.1038/s41587-024-02133-2](https://doi.org/10.1038/s41587-024-02133-2)

---

## Overview

**De novo 단백질 설계**의 역사와 최신 딥러닝 기반 방법론을 종합 정리한 리뷰. 단백질 설계의 "중심 교리"—원하는 기능 → 구조 설계 → 서열 탐색—를 바탕으로, 전통적 물리 기반 방법부터 최신 딥러닝 구조 설계 모델까지의 발전 과정을 서술한다. 특히 구조 설계(fold design)에서 기능 설계(function design)로의 패러다임 전환을 조명하며, 항체, 효소, 백신 항원 등 실용적 응용 사례를 다룬다.

---

## Key Topics

**전통적 단백질 설계 방법**
- 물리 기반(energy function) 방법: Rosetta 등 원자 수준 에너지 계산으로 서열 탐색
- PDB 데이터 기반 단편 조립(fragment assembly)으로 새로운 폴드 설계
- 한계: 고차원 서열 공간 탐색의 계산 비용, 에너지 함수의 정확도 한계

**딥러닝 기반 구조 설계 혁신**
- ProteinMPNN, RFdiffusion, ESMFold 등 딥러닝 기반 역폴딩(inverse folding) 및 구조 생성 모델
- AlphaFold2와의 결합으로 설계된 서열의 구조 예측 정밀도 급상승 → 실험적 검증 성공률 향상
- 이전에는 α-헬릭스 번들 위주였으나, 이제 β-sheet 포함 다양한 구조 설계 가능

**기능 설계로의 확장**
- 리간드/기질 결합 부위 설계: 원하는 결합 형태를 먼저 정의 후 이를 지지하는 구조 생성
- 효소 활성 부위 de novo 설계: Kemp eliminase 등 자연에 존재하지 않는 촉매 반응 구현
- 항체 CDR 루프 설계, 나노입자 자가조립체(nanoparticle) 설계
- 단백질-단백질 상호작용 인터페이스 설계

**구조·서열 공동 설계 및 유연성 제어**
- 서열과 구조를 동시에 최적화하는 co-design 방법론 대두
- 구조적 유연성(flexibility) 및 알로스테릭 제어를 설계에 통합하는 방향

---

## Key Findings

- 딥러닝 기반 구조 설계 모델은 전통 물리 기반 방법 대비 성공률을 수십 배 향상
- RFdiffusion + ProteinMPNN 파이프라인이 현재 de novo 단백질 설계의 실질적 표준
- 기능적 단백질(효소, 항체, 결합 단백질) 설계가 이제 "개념 증명"을 넘어 실용화 단계에 진입
- 여전히 β-sheet 주도 복잡한 폴드 및 다중 도메인 단백질 설계는 미해결 과제
- 구조적 유연성과 알로스테릭 전달을 설계에 통합하는 것이 차세대 도전

---

## Perspective

De novo 단백질 설계는 딥러닝으로 인해 "가능성"에서 "적용"으로 이동 중이다. 백신 항원(mRNA 백신용 안정화 Spike 단백질), 신약(효소 치료제), 소재(자가조립 나노구조체) 등 분야에서 실질적 영향이 기대된다. 향후 도전 과제는 복잡한 활성 부위를 가진 효소 설계, 다구조 단백질의 유연성 제어, 그리고 설계-합성-검증의 폐쇄 루프 자동화이다.

---

## Key References

- Jumper J et al. (2021) Highly accurate protein structure prediction with AlphaFold. *Nature* 596:583-589. [doi:10.1038/s41586-021-03819-2](https://doi.org/10.1038/s41586-021-03819-2)
- Watson JL et al. (2023) De novo design of protein structure and function with RFdiffusion. *Nature* 620:1089-1100. [doi:10.1038/s41586-023-06415-8](https://doi.org/10.1038/s41586-023-06415-8)
- Dauparas J et al. (2022) Robust deep learning-based protein sequence design using ProteinMPNN. *Science* 378:49-56. [doi:10.1126/science.add2187](https://doi.org/10.1126/science.add2187)
- Notin P et al. (2024) Machine learning for functional protein design. *Nat Biotechnol* 42:216-228. [doi:10.1038/s41587-024-02127-0](https://doi.org/10.1038/s41587-024-02127-0)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
