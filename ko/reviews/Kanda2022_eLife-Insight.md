# Implementing robotics and artificial intelligence (eLife Insight)

## Citation (NLM)
Sebastian S. Implementing robotics and artificial intelligence. eLife. 2022;11:e80609. doi: 10.7554/eLife.80609

**DOI:** [https://doi.org/10.7554/eLife.80609](https://doi.org/10.7554/eLife.80609)

---

## Overview

Kanda et al. (2022, eLife)의 **LabDroid + Bayesian 최적화** 연구를 소개하는 eLife Insight 논평. 로봇과 AI를 결합하여 재생의학용 세포배양 프로토콜을 자동 최적화한 접근의 의미를 일반 독자 수준으로 설명한다. 인간 조작자의 개입을 최소화하고 물리적 파라미터(피펫팅 강도, 세포 분리 시간 등)까지 최적화 대상에 포함시킨 점에서 기존 자동화와 차별화된다.

---

## Key Topics

**재생의학에서의 세포배양 문제**
- 줄기세포 분화 프로토콜은 복잡하고 조작자 의존성이 높아 재현성 확보가 어려움
- 세포는 환경 자극(물리적·화학적)에 민감하여 표준화 어려움
- 임상 적용을 위한 세포 품질 기준이 엄격하고 점점 높아지는 추세

**LabDroid 로봇 자동화 접근**
- Humanoid 로봇 팔(Maholo)이 실험자 역할을 대체, 물리적 파라미터를 정밀 재현
- 로봇은 동일 작업을 오차 없이 반복 가능 → 물리적 변수를 실험 변수로 체계적 탐색 가능
- iPSC → RPE 분화의 7개 파라미터(화학·물리 혼합) 공간을 배치 Bayesian 최적화(BBO)로 탐색

**결과 및 의의**
- 111일, 143회 조건 탐색으로 baseline 대비 착색 면적 비율(RPE 분화 지표) 88% 향상
- 로봇 시스템이 인간 조작자보다 높은 재현성과 데이터 추적성(traceability) 확보
- 선행 연구 인용: Imai et al. (2018) 이미징 기반 품질 평가, Simon et al. (2016) 세포치료 품질 표준, Sebastian et al. (2019) 공정 개발 리스크 관리

---

## Key Findings

- 로봇의 물리적 파라미터 재현성이 세포 분화 효율에 유의하게 기여
- BBO는 고차원 파라미터 공간에서 적은 실험 수로 효율적인 최적화 달성
- 이 접근은 다른 세포 유형 분화, 약물 스크리닝, 조직 공학 등에 광범위하게 적용 가능

---

## Perspective

LabDroid와 같은 범용 로봇 + AI 최적화 시스템은 재생의학 제조 자동화의 패러다임을 바꿀 수 있다. 향후 과제는 다목적 함수 최적화(착색도 외 유전자 발현, 기능 지표 포함), 다양한 세포 유형으로의 확장, 그리고 GMP(우수 의약품 제조 관리 기준) 환경에서의 검증이다.

---

## Key References

- Kanda GN et al. (2022) Robotic search for optimal cell culture in regenerative medicine. *eLife* 11:e77007. [doi:10.7554/eLife.77007](https://doi.org/10.7554/eLife.77007)
- Imai M et al. (2018) Automatic quality control system of cell manufacturing for corneal endothelial cells. *Regen Ther* 9:70-76. [doi:10.1016/j.reth.2018.08.002](https://doi.org/10.1016/j.reth.2018.08.002)
- Simon CG et al. (2016) Strategies for achieving measurement assurance for cell therapy products. *Stem Cells Transl Med* 5(6):705-708. [doi:10.5966/sctm.2015-0269](https://doi.org/10.5966/sctm.2015-0269)
- Sebastian S et al. (2019) The management of risk and investment in cell therapy process development. *Regen Med* 14(5):465-488. [doi:10.2217/rme-2018-0081](https://doi.org/10.2217/rme-2018-0081)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
