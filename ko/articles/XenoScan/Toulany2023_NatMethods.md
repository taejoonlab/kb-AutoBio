# Uncovering developmental time and tempo using deep learning

## Citation (NLM)
Toulany N, Morales-Navarrete H, Čapek D, Grathwohl J, Ünalan M, Müller P. Uncovering developmental time and tempo using deep learning. Nat Methods. 2023;20:2000-2010. doi: 10.1038/s41592-023-02083-8

**DOI:** [https://doi.org/10.1038/s41592-023-02083-8](https://doi.org/10.1038/s41592-023-02083-8)

---

## Background
- 동물 발생은 수정란에서 성체까지 복잡한 형태학적 변화 거쳐, 종 간 발생 속도(tempo) 차이가 진화적 신규성 주요 동인으로 부상
- 기존 발생 단계(staging)는 수동 현미경 관찰에 의존, 이상화된 staging atlas는 개체 간 변이·부드러운 단계 전이 반영 못 함
- Deep learning으로 배아 이미지 간 유사도 자동·unbiased 계산, 발생 시간·tempo 정량화 필요

## Key Experiment Methods
1. **Deep learning 기반 유사도 계산**: 서로 다른 시간대 배아 이미지 간 유사도 자동 계산, complex phenotypic fingerprints 도출
2. **발생 시간·tempo 정량화**: 단계 간 유사도로 developmental time과 tempo 정량적 결정, 온도 의존적 발생 속도 측정
3. **Unsupervised staging atlas 유도**: 다수 종의 staging atlas를 de novo·unsupervised manner로 자동 생성
4. **개별 배아 발생 진행 추적**: 자연 발생·유도된 변화 감지, 개별 배아 수준에서 발생 진행 정량화
5. **최적화 파라미터**: CNN 아키텍처, similarity metric, timestamp 해상도, 종 간 비교 기준, unsupervised clustering 알고리즘

## Results
- Deep learning이 배아 staging을 높은 정확도로 자동 수행
- 온도 의존적 발생 tempo 정량적 결정 성공
- 자연 발생 및 유도된 변화(신호전달 억제 등)로 인한 발생 진행 변화 개별 배아 수준에서 감지
- 다수 종의 staging atlas를 de novo unsupervised 방식으로 유도
- Phenotypic fingerprints가 발생 시간·tempo에 대한 특징적 정보 운반
- 객관적·표준화된 초기 발생 분석 방법론 정립

## Perspective
- Deep learning 기반 발생 staging이 수동 관찰의 한계 해소, 표준화된 분석 제공
- 종 간 발생 tempo 비교가 진화 발생학(evo-devo) 연구에 기여
- Unsupervised staging atlas 유도가 비모델 생물의 발생 연구 접근성 향상
- 환경 요인(온도, 화학 물질)이 발생 속도에 미치는 영향 정량적 평가 가능
- 향후 다중 종·다중 조건 발생 비교로 진화적 형태 형성 기전 규명

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
