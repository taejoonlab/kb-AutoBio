# Opportunities and challenges in design and optimization of protein function

## Citation (NLM)
Listov D, Goverde CA, Correia BE, Fleishman SJ. Opportunities and challenges in design and optimization of protein function. Nat Rev Mol Cell Biol. 2024;25(8):639-653. doi: 10.1038/s41580-024-00718-y

**DOI:** [https://doi.org/10.1038/s41580-024-00718-y](https://doi.org/10.1038/s41580-024-00718-y)

---

## Overview

단백질 기능 **최적화(optimization)**와 **de novo 설계(de novo design)**를 아우르는 최신 방법론 리뷰. 구조 기반(structure-based) 원자 수준 계산과 서열 기반(sequence-based) 머신러닝 방법을 어떻게 조합하여 단백질 공학의 신뢰성을 높였는지 체계적으로 정리한다. 특히 치료제(항체, 백신 항원), 효소(녹색 화학, 치료적 효소), 약물 전달 나노구조체 등 실용적 응용에 방법론을 연결하는 점에서 실용적 가이드로 기능한다.

---

## Key Topics

**단백질 최적화 (자연 단백질 개선)**
- 안정성 설계(Stability design): 열역학적 원리(positive/negative design)로 native state 안정화
  - 웹 서버로 구현된 자동화 도구(FoldX, Rosetta 등)로 소수 설계로 유의미한 안정성 향상
  - 사례: Plasmodium falciparum RH5 항원 안정화(E.coli 생산 가능, 열안정성 15°C 향상), SARS-CoV-2 Spike 안정화(11배 향상된 발현, 중화 항체 역가 향상)
  - AlphaFold2 도입으로 실험 구조 없이도 설계 가능 단백질 범위 급확장
- 활성·특이성 최적화: 에너지 계산 + 진화적 서열 보존 정보 통합(phylogenetic constraints)

**De Novo 단백질 설계**
- 고전적 방법: Rosetta 기반 fragment assembly로 자연에 없는 새 폴드 설계
- 딥러닝 세대: 
  - 역폴딩(Inverse folding): ProteinMPNN 등으로 원하는 구조에 맞는 서열 생성
  - 확산 모델(Diffusion model): RFdiffusion으로 기능 부위를 고정하고 주변 구조를 생성
  - 언어 모델(Language model): ESM 등으로 서열 공간에서 새로운 기능성 서열 탐색
- 현재 한계: α-헬릭스 번들 중심 → β-sheet 주도 복잡한 폴드로의 확장이 주요 과제

**치료 및 산업 응용**
- 백신 항원: Spike 안정화, RSV F 단백질, malaria RH5 등
- 효소: Chondroitinase ABC 안정화(기능적 반감기 6일 이상), 녹색 화학용 산업 효소
- 항체: CDR 최적화, 결합 특이성·친화도 개선
- 나노구조체: 약물 전달용 자가조립 단백질 케이지

---

## Key Findings

- 원자 수준 설계 + 계통발생학적 서열 제약을 결합하면 negative design 문제(경쟁 misfolded states 억제)를 효과적으로 해결
- AlphaFold2 등장으로 실험적으로 결정된 구조 없는 단백질도 안정성 설계 가능, 적용 범위가 PDB 20만 개 → 게놈 데이터베이스 수억 개 서열로 확장
- 딥러닝 모델(RFdiffusion + ProteinMPNN)이 기능적 단백질 de novo 설계의 실질적 표준으로 자리잡음
- α-헬릭스 번들 이상의 복잡한 폴드(복잡한 활성 부위 포함 효소) 설계는 여전히 도전적
- 막단백질 설계 방법론도 최근 등장하여 주요 신약 타깃으로 활용 기대

---

## Perspective

단백질 설계는 이제 "자연이 진화시킨 것"의 한계를 넘어 "자연에 없는 기능"을 처음부터 설계하는 방향으로 진화하고 있다. 특히 글로벌 감염병 대응(빠른 백신 항원 설계), 만성질환 치료(효소 치료제), 지속 가능한 화학(생촉매) 분야에서 파급력이 클 것으로 예상된다. 향후 관건은 더 복잡한 폴드 설계, 다중 기능(multifunctional) 단백질 설계, 그리고 설계-합성-검증의 자동화 루프 완성이다.

---

## Key References

- Jumper J et al. (2021) Highly accurate protein structure prediction with AlphaFold. *Nature* 596:583-589. [doi:10.1038/s41586-021-03819-2](https://doi.org/10.1038/s41586-021-03819-2)
- Watson JL et al. (2023) De novo design of protein structure and function with RFdiffusion. *Nature* 620:1089-1100. [doi:10.1038/s41586-023-06415-8](https://doi.org/10.1038/s41586-023-06415-8)
- Dauparas J et al. (2022) Robust deep learning-based protein sequence design using ProteinMPNN. *Science* 378:49-56. [doi:10.1126/science.add2187](https://doi.org/10.1126/science.add2187)
- Chu AE et al. (2024) Sparks of function by de novo protein design. *Nat Biotechnol* 42:203-215. [doi:10.1038/s41587-024-02133-2](https://doi.org/10.1038/s41587-024-02133-2)
- Notin P et al. (2024) Machine learning for functional protein design. *Nat Biotechnol* 42:216-228. [doi:10.1038/s41587-024-02127-0](https://doi.org/10.1038/s41587-024-02127-0)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
