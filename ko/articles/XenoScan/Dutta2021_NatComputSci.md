# Machine learning-guided directed evolution of enzymes

## Citation (NLM)
Dutta A, et al. Cluster learning-assisted directed evolution. Nat Comput Sci. 2021;1:815-825. doi: 10.1038/s43588-021-00110-2

**DOI:** [https://doi.org/10.1038/s43588-021-00110-2](https://doi.org/10.1038/s43588-021-00110-2)

---

## Background
- Directed evolution이 효소 공학의 핵심이나, fitness landscape 탐색이 실험 비용·시간 소모적
- ML이 서열-기능 관계 학습으로 탐색 공간 축소, 활성 변이체 예측 효율화
- Clustering 기반 학습이 fitness 이질성 식별, informative training set 사전선택
- Self-driving lab 개념이 효소 최적화 전 과정 자동화에 적용

## Key Experiment Methods
1. **ML-guided directed evolution**: 서열-기능 데이터로 surrogate 모델 학습, acquisition function으로 다음 실험 우선순위 결정
2. **Clustering-assisted training**: unsupervised clustering으로 fitness landscape partitioning, 대표 서열 선택으로 실험 부담 최소화
3. **Zero-shot predictor**: 실험 없이 fitness 예측하는 unsupervised 모델로 training set selection 제한
4. **Greedy search 최적화**: 학습된 모델로 가상 landscape 탐색, minimal experiment로 global optimum 접근
5. **최적화 파라미터**: 모델 아키텍처, clustering 알고리즘, training set 크기, acquisition function, iteration 수

## Results
- ML-guided directed evolution이 기존 DE 대비 실험 횟수 대폭 감소 while maintaining or improving fitness
- Clustering-assisted training이 fitness 이질성 효과적으로 식별, small informative subset으로 모델 학습
- Zero-shot predictor가 실험 없이 유망 변이체 사전 선별
- Minimal experiment iteration으로 효소 활성·안정성·선택성 최적화
- Self-driving lab 개념이 효소 공학 파이프라인에 성공적으로 적용

## Perspective
- ML + directed evolution 통합이 효소 공학의 처리량·속도 획기적 개선
- Clustering 기반 학습이 고차원 fitness landscape 탐색 효율화
- Self-driving enzyme engineering 플랫폼이 산업 생명공학·의약품 생산에 광범위 적용
- 향후 다중 목적 최적화, 대사 경로 최적화, new-to-nature 반응 설계로 확장
- 자동화 DE 플랫폼이 합성생물학 핵심 인프라로 발전

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
