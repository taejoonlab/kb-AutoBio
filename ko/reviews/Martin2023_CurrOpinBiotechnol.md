# Perspectives for self-driving labs in synthetic biology

## Citation (NLM)
Martin HG, Radivojevic T, Zucker J, Bouchard K, Sustarich J, Peisert S, Arnold D, Hillson N, Babnigg G, Marti JM, Mungall CJ, Beckham GT, Waldburger L, Carothers J, Sundaram S, Agarwal D, Simmons BA, Backman T, Banerjee D, Tanjore D, Ramakrishnan L, Singh A. Perspectives for self-driving labs in synthetic biology. Curr Opin Biotechnol. 2023;79:102881. doi: 10.1016/j.copbio.2022.102881

**DOI:** [https://doi.org/10.1016/j.copbio.2022.102881](https://doi.org/10.1016/j.copbio.2022.102881)

---

## Overview

화학·소재 분야에서 주로 발전한 **Self-Driving Labs (SDLs)**를 **합성생물학(synthetic biology)**으로 확장할 때의 기회와 도전을 논의하는 관점 논문. 게놈 DNA가 세포 표현형의 단일 저장소(single repository)라는 생물학적 특수성이 SDL 구현에 독특한 기회를 제공하는 동시에, 생물학적 시스템의 복잡성·적응성이 특유의 기술적 도전을 만든다는 점을 분석한다. Lawrence Berkeley 국립연구소 등 미국 주요 연구기관 공동 저술.

---

## Key Topics

**SDL의 정의와 자율성 수준 (Autonomy Levels)**
- SDL = 자동화 실험(로봇) + AI 의사결정(실험 설계·가설 검증)의 폐쇄 루프
- 자율성 0~5 단계 분류:
  - Level 0: 전 과정 인간 수동 수행
  - Level 1: 반복 작업 일부 로봇화
  - Level 2: 프로토콜·데이터의 기계 가독성 디지털화 (예: Aquarium LIMS)
  - Level 3 이상 = 진정한 SDL (Design–Build–Test–Learn 자동 루프)
  - Level 4: 로봇이 실험 실행·일상 분석 담당, 인간은 목표 설정만 (예: Adam, Eve 로봇 과학자)
  - Level 5: 인간은 목표 제시, 로봇이 독립적 연구 수행

**합성생물학 SDL의 기회**
- 게놈 편집 기술(CRISPR 등)로 세포 표현형 조작을 단일 표적(DNA)에 집중 가능
- 진화가 만든 다양한 표현형 공간을 SDL로 탐색하면 획기적 생물 기반 화학물질(바이오연료, 의약품) 생산 가능
- 예시: bisabolene 바이오연료 생산 경로 최적화를 위한 자동화 DNA 조립 + AI 추천 루프

**합성생물학 SDL의 도전**
- **생물학적 복잡성**: 생명체는 환경·유전체 상호작용이 복잡하여 화학 반응처럼 단순 파라미터화 어려움
- **적응성 문제**: 세포는 실험 중 진화하거나 예측 불가한 방식으로 반응 → 재현성 저하
- **측정 지연**: 생물학적 표현형 측정(발현, 대사물 분석)은 화학 분석보다 시간 소요 큼
- **데이터 표준화 부재**: 생물학 실험 프로토콜·데이터의 기계 가독성 표준이 부족
- **대규모 투자 필요**: 생물학 SDL 구축 비용이 화학 SDL 대비 높음

**기존 생물학 SDL 사례**
- Adam, Eve (2009, 2010): 효모 유전자 기능·항말라리아 약물 탐색 로봇 과학자
- BioAutomata: E. coli의 lycopene 생산을 위한 프로모터 최적화 자동화 플랫폼
- Kanda et al. (2022): 로봇 + Bayesian 최적화로 줄기세포 분화 최적 조건 탐색

---

## Key Findings

- 생물학 SDL은 화학 SDL 대비 기술 성숙도가 낮으나 잠재적 응용 가치는 훨씬 큼
- 완전 자율화(Level 5) 이전에 Level 3~4 시스템을 목표로 단계적 구현이 현실적
- 대용량 고품질 데이터 생산 능력이 AI 모델의 효과를 결정하며, SDL이 이를 가능하게 함
- 24/7 운전과 선형 확장성(장비 추가)이 인간 기반 연구 대비 SDL의 핵심 우위
- 투자 정당성 확보를 위해 SDL은 난이도 높고 임팩트 있는 생물학적 문제를 대상으로 해야 함

---

## Perspective

합성생물학 SDL은 바이오연료, 의약품, 산업 효소의 미생물 생산 최적화에서 가장 빠른 실용화가 기대된다. 단기 과제는 생물학 실험 프로토콜의 디지털화 표준 확립과 생물학적 데이터 기계 가독성 향상이며, 중장기적으로는 세포 적응(진화)을 실험 루프에 통합하는 방법론 개발이 필요하다.

---

## Key References

- Abolhasani M, Kumacheva E (2023) The rise of self-driving labs in chemical and materials sciences. *Nat Synth* 2:483-492. [doi:10.1038/s44160-022-00231-0](https://doi.org/10.1038/s44160-022-00231-0)
- King RD et al. (2009) The automation of science. *Science* 324:85-89. [doi:10.1126/science.1165620](https://doi.org/10.1126/science.1165620) (Adam 로봇 과학자)
- Beal J, Rogers MF (2020) Levels of autonomy in synthetic biology engineering. *ACS Synth Biol* [doi:10.1021/acssynbio.9b00514](https://doi.org/10.1021/acssynbio.9b00514)
- Kanda GN et al. (2022) Robotic search for optimal cell culture in regenerative medicine. *eLife* 11:e77007. [doi:10.7554/eLife.77007](https://doi.org/10.7554/eLife.77007)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
