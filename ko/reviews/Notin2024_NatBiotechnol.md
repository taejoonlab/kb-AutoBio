# Machine learning for functional protein design

## Citation (NLM)
Notin P, Rollins N, Gal Y, Sander C, Marks D. Machine learning for functional protein design. Nat Biotechnol. 2024;42(2):216-228. doi: 10.1038/s41587-024-02127-0

**DOI:** [https://doi.org/10.1038/s41587-024-02127-0](https://doi.org/10.1038/s41587-024-02127-0)

---

## Overview

기능적 단백질 설계(functional protein design)에 적용되는 머신러닝(ML) 방법론을 통합된 프레임워크로 정리한 리뷰. **서열(sequence), 구조(structure), 기능 레이블(functional label)**의 세 가지 핵심 데이터 양식(modality)에 기반하여 ML 모델을 분류하고, 각 접근이 효소, 항체, 백신, 나노머신 등 실용적 설계 과제에 어떻게 적용되는지를 체계적으로 논의한다.

---

## Key Topics

**세 가지 핵심 데이터 양식**
- **서열(Sequence)**: 수십억 개 공개 단백질 서열 → 진화적 제약 학습; 서열만으로 fitness landscape 모델링
- **구조(Structure)**: PDB의 3D 구조 데이터 → 원자 수준 상호작용 학습; fold design, 결합 부위 설계
- **기능 레이블(Functional label)**: 실험실 생성 돌연변이-표현형 데이터(DMS, 고처리량 선택 실험) → 새로운 기능 설계에 직접 활용

**설계 목표의 세 가지 유형**
1. **기존 기능 강화 (Redesign to enhance)**: 안정성·친화도·특이성 등 기존 기능 개선 → 주로 서열 모델 활용 (EVE, ESM, Tranception 등)
2. **새 기능으로 재설계 (Redesign for new function)**: 기존 단백질에서 출발하여 다른 기질/표적에 작용 → 서열-레이블 모델 활용, DMS 데이터 기반
3. **De novo 설계**: 처음부터 새로운 폴드와 기능 설계 → 서열-구조 모델(ProteinMPNN, RFdiffusion) 주도

**ML 모델 유형**
- **서열 기반 모델**: 서열만으로 훈련; MSA 기반 진화적 모델(EVE, ESM-1v), 자기회귀 언어 모델(ProGen, ESM-3)
- **서열-구조 모델**: 3D 구조 정보 포함; 역폴딩 모델(ProteinMPNN), 확산 모델(RFdiffusion)
- **서열-레이블 모델**: 실험적 돌연변이-기능 데이터로 훈련; 지도 학습 기반, 새 기능 설계에 특화

**실용적 응용 분야**
- 효소: 새로운 반응 특이성, 열안정성 개선, 새 기질 범위
- 항체: CDR 최적화, 면역원성 감소, 중화 항체 폭 확장
- 백신 항원: 바이러스 항원 안정화, 브로드 스펙트럼 면역 유도
- 나노머신·자가조립 단백질: 약물 전달, 나노소재

**향후 트렌드**
- 대규모 실험(DMS, NGS 기반 선택) + 자동화 실험실 → 훈련 데이터 대폭 확대
- 멀티모달 기반 모델(foundation model)로 서열·구조·기능을 통합 학습
- 강화학습(RL) + 실험 자동화 결합으로 설계-검증 루프 단축
- 표준화된 벤치마크 데이터셋 필요성 강조

---

## Key Findings

- 서열 기반 모델은 DMS 데이터 예측에서 물리 기반 방법을 능가하며, 대규모 서열 데이터로 훈련할수록 성능 향상
- 서열-구조 모델(ProteinMPNN 등)은 안정적인 새 단백질 서열 생성에 현재 최고 성능
- 기능 레이블 데이터가 제한적일 때는 서열 기반 모델이, 충분할 때는 서열-레이블 모델이 유리
- de novo 설계에서 ML은 α-헬릭스 번들을 넘어 β-sheet 포함 다양한 폴드로 확장 중
- 단일 모달리티 한계를 넘어 멀티모달 통합이 향후 주요 방향

---

## Perspective

ML 기반 단백질 설계는 "fitness landscape 탐색"의 효율을 혁명적으로 높였다. 현재 가장 큰 병목은 다양한 기능적 맥락에서 생성된 대규모·고품질 실험 데이터의 부족이다. 대규모 자동화 실험(자율 실험실, 고처리량 선택)과 ML의 결합이 이 병목을 해소하면 단백질 공학의 속도와 범위는 또 한 번 도약할 것으로 전망된다.

---

## Key References

- Notin P et al. (2022) Tranception: protein fitness prediction with autoregressive transformers and inference-time retrieval. *ICML 2022* [doi:10.48550/arXiv.2205.13760](https://doi.org/10.48550/arXiv.2205.13760)
- Jumper J et al. (2021) Highly accurate protein structure prediction with AlphaFold. *Nature* 596:583-589. [doi:10.1038/s41586-021-03819-2](https://doi.org/10.1038/s41586-021-03819-2)
- Dauparas J et al. (2022) Robust deep learning-based protein sequence design using ProteinMPNN. *Science* 378:49-56. [doi:10.1126/science.add2187](https://doi.org/10.1126/science.add2187)
- Listov D et al. (2024) Opportunities and challenges in design and optimization of protein function. *Nat Rev Mol Cell Biol* 25:639-653. [doi:10.1038/s41580-024-00718-y](https://doi.org/10.1038/s41580-024-00718-y)
- Chu AE et al. (2024) Sparks of function by de novo protein design. *Nat Biotechnol* 42:203-215. [doi:10.1038/s41587-024-02133-2](https://doi.org/10.1038/s41587-024-02133-2)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
