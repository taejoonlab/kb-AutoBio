# Cluster learning-assisted directed evolution

## Citation (NLM)
Qiu Z, Wu R, Wang Y, Wei G. Cluster learning-assisted directed evolution. Nat Comput Sci. 2021;1:815-825. doi: 10.1038/s43588-021-00168-y

**DOI:** [https://doi.org/10.1038/s43588-021-00168-y](https://doi.org/10.1038/s43588-021-00168-y)

---

## Background
- Directed evolution(DE)은 자연선택 모방으로 단백질 특성 개선, fitness 평가는 비용·시간 소모적
- Fitness landscape는 고차원 표면으로 아미노산 서열을 활성·선택성·안정성 등에 매핑, epistasis로 인해 greedy search는 국소 최적점에 제한
- Multi-site-saturation mutagenesis는 방대한 조합 라이브러리로 스크리닝 용량 초과
- ML-assisted directed evolution(MLDE)이 active learning으로 surrogate model + acquisition function 조합 사용
- CLADE(Cluster Learning-Assisted Directed Evolution) 프레임워크: unsupervised clustering으로 training set 사전선택, fitness 이질성 식별

## Key Experiment Methods
1. **Unsupervised clustering 전략**: self-supervised protein embedding(variational autoencoder, transformer 등)으로 서열 특징 추출, clustering으로 fitness 이질성 있는 subspace 분할
2. **Training set 사전선택**: 각 cluster에서 대표 서열 선택, small informative subset으로 supervised 모델 학습 - 실험 부담 최소화(2회 iteration)
3. **Zero-shot predictor 활용**: 실험 없이 fitness 예측하는 unsupervised predictor로 training set selection 제한
4. **Surrogate model + greedy search**: 학습된 모델로 fitness landscape 가상 탐색, greedy search로 단백질 fitness 최적화
5. **CLADE 프레임워크 검증**: 효소 진화(활성·선택성 개선), 형광 단백질, 단백질 안정성 최적화 등 다양한 시스템 적용
6. **최적화 파라미터**: clustering 알고리즘 선택, cluster 수, embedding 모델, training set 크기, acquisition function, iteration 수

## Results
- Unsupervised clustering으로 fitness 이질성 식별 성공, cluster 간 fitness 분포 명확히 차별화
- Small informative subset(전체 라이브러리의 일부)으로 supervised 모델 학습, 실험 부담 2회 iteration으로 최소화
- CLADE가 기존 MLDE 대비 state-of-the-art 결과 달성, 동일 실험 횟수에서 더 높은 fitness 변이 발견
- Epistatic landscape에서 효과적 탐색, greedy search의 국소 최적점 문제 해결
- 다양한 단백질 시스템(효소, 형광 단백질, 안정성 최적화)에서 일반화 성능 확인
- Self-supervised embedding이 방대한 비라벨 서열 데이터에서 잠재 생물정보 포획, downstream task 전달

## Perspective
- Unsupervised clustering + supervised learning 통합이 MLDE 효율성 획기적 개선
- Self-supervised protein embedding이 단백질 공학의 핵심 도구로 정립
- CLADE 프레임워크가 실험 부담 최소화하면서 고 fitness 변이 효율적 발견
- 향후 다중 목적 최적화(활성+안정성+선택성), 대사 경로 최적화로 확장
- 자동화 DE 플랫폼과 결합하여 self-driving protein engineering 실현

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
