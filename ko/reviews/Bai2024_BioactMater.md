# AI-enabled organoids: Construction, analysis, and application

## Citation (NLM)
Bai L, Wu Y, Li G, Zhang W, Zhang H, Su J. AI-enabled organoids: Construction, analysis, and application. Bioact Mater. 2024;31:525-548. doi: 10.1016/j.bioactmat.2023.09.005

**DOI:** [https://doi.org/10.1016/j.bioactmat.2023.09.005](https://doi.org/10.1016/j.bioactmat.2023.09.005)

---

## Overview

**AI-Enabled Organoids**라는 개념을 제안하고, 오가노이드 연구의 세 핵심 단계(구축 전략, 데이터 분석, 전임상 적용)에 AI가 어떻게 기여할 수 있는지를 종합 정리한 리뷰. 오가노이드 연구의 현실적 병목—매트릭스 소재·배양 조건·성장인자의 광범위한 조합 탐색, 고해상도 다초점 이미징 데이터 분석, 멀티오믹스 통합—에 AI를 접목하는 다양한 접근법을 소개한다.

---

## Key Topics

**오가노이드 구축 전략에서 AI의 역할**
- 세포외 기질(ECM) 소재 최적화: 탄성률, 기공도, 분해성 조합 탐색에 AI 보조
- 배양 조건 최적화: 온도, CO2, 성장인자 농도(Wnt, BMP 등) 조합에 베이지안 최적화 또는 강화학습 적용
- 고비용·저효율의 문헌 추론 + in vitro 실험 반복 사이클을 AI 기반 능동학습(active learning)으로 대체

**AI 기반 이미징 분석**
- 멀티포컬 3D 이미징 데이터의 이질성(heterogeneity) 분석
- 딥러닝(CNN 계열) 기반 자동 형태 분류, 세포 계수, 조직 구조 정량화
- 비표지(label-free) 이미징 + AI 분류를 통해 형광 표지 없이 세포 유형 동정

**멀티오믹스 데이터 분석**
- 단일세포 전사체(scRNA-seq), 유전체, 대사체 등 멀티오믹스 통합
- 그래프 신경망(GNN), 변분 오토인코더(VAE) 등을 이용한 다차원 데이터의 의미 있는 임베딩
- 세포 궤적 분석, 발달 경로 추론

**전임상 평가 및 적용**
- 약물 스크리닝: 오가노이드 반응성 AI 분류로 신약 후보 우선순위 결정
- 종양 오가노이드: 환자 맞춤형 화학요법 반응 예측
- 재생의학: 이식 전 오가노이드 품질 AI 검증

---

## Key Findings

- AI가 오가노이드 매트릭스 소재 조성과 성장인자 조합 최적화 실험 수를 대폭 감소시킴
- 딥러닝 기반 이미징 분석은 숙련 연구자의 수동 분석과 비교할 만한 정확도 달성
- 멀티오믹스 AI 분석으로 오가노이드의 발달 경로 및 세포 아형을 고해상도로 규명 가능
- 환자 유래 종양 오가노이드 + ML 약물 반응 예측은 임상에서의 정밀의료 실현 가능성 제시
- 현재 주요 한계: 오가노이드 배치(batch) 간 변동성이 AI 모델 훈련 데이터 품질에 영향

---

## Perspective

AI-Enabled Organoids는 기초 연구에서 임상 적용까지의 파이프라인을 단축할 수 있는 유망한 접근이다. 특히 개인 맞춤 의학(personalized medicine)과 재생의학의 실용화에 AI가 핵심 역할을 할 것으로 전망된다. 향후 과제는 오가노이드 표준화(재현성 향상), 멀티모달 AI 모델 고도화, 그리고 실제 임상 데이터와의 통합 검증이다.

---

## Key References

- Lancaster MA, Knoblich JA (2014) Organogenesis in a dish: modeling development and disease using organoid technologies. *Science* 345:1247125. [doi:10.1126/science.1247125](https://doi.org/10.1126/science.1247125)
- Huch M et al. (2017) The hope and the hype of organoid research. *Development* 144:938-941. [doi:10.1242/dev.150201](https://doi.org/10.1242/dev.150201)
- LeCun Y, Bengio Y, Hinton G (2015) Deep learning. *Nature* 521:436-444. [doi:10.1038/nature14539](https://doi.org/10.1038/nature14539)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
