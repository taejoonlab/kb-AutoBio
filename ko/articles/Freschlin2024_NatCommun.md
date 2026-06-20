# Neural network extrapolation to distant regions of the protein fitness landscape

## Citation (NLM)
Freschlin CR, Fahlberg SA, Heinzelman P, Romero PA. Neural network extrapolation to distant regions of the protein fitness landscape. Nat Commun. 2024;15:6405. doi: 10.1038/s41467-024-50712-3

**DOI:** [https://doi.org/10.1038/s41467-024-50712-3](https://doi.org/10.1038/s41467-024-50712-3)

---

## Background
- ML이 단백질 공학에서 서열-기능 관계 모델 구축으로 신규 생체분자 발견 가속화
- ML 가이드 단백질 설계는 국소 서열-기능 데이터로 학습한 모델이 원격 fitness peak를 정확히 예측해야 함
- 신경망의 학습 데이터 외부 extrapolation 능력 평가 필요
- 단백질 G(GB1)-IgG 결합 데이터로 모델 가이드 설계, 수천 개 GB1 변이 실험적 검증으로 extrapolation 체계적 평가

## Key Experiment Methods
1. **신경망 아키텍처 패널**: 선형 모델, MLP, CNN, transformer 등 다양한 아키텍처로 동일 데이터 학습, 각 모델의 귀납적 편향(inductive bias)이 학습하는 landscape 양상 비교
2. **모델 가이드 in silico 탐색**: ML 모델로 서열-기능 landscape 탐색, 수천 개 GB1 변이 설계(학습 영역 벗어난 방대한 서열 공간 샘플링)
3. **고속 yeast display assay**: 설계된 GB1 변이 수천 개 실험적 검증, IgG 결합 기능 측정, 모델 예측과 실험 결과 비교
4. **Extrapolation 평가**: local extrapolation(학습 데이터 근처) vs distant extrapolation(서열 공간 깊은 영역) 성능 비교
5. **앙상블 접근법**: CNN.simple ensemble로 robust design 달성, 개별 모델의 design preference 통합
6. **최적화 파라미터**: 모델 아키텍처 선택, 학습 데이터 크기, 돌연변이 수, 서열 위치, 아미노산 치환 유형, ensemble 구성

## Results
- 각 모델 아키텍처가 동일 데이터에서 현저히 다른 landscape 추론, 고유 design preference 발생
- 단순 모델(linear, shallow MLP)이 local extrapolation에서 우수 - 고 fitness 단백질 설계 성공
- 정교한 CNN이 서열 공간 깊이 탐색 가능하지만 접히는 단백질 설계는 가능하나 기능 상실
- CNN simple ensemble이 local landscape에서 고성능 변이 robust 설계 가능
- 모델의 귀납적 편향이 단백질 fitness landscape의 서로 다른 측면 학습에 영향
- 실험적 검증으로 ML 모델 예측력 체계적 벤치마크 최초 수행

## Perspective
- 단백질 공학에서 모델 아키텍처 선택이 설계 전략에 결정적 영향
- Ensemble 접근법이 단일 모델 한계 보완, 단백질 공학 robustness 향상
- Distant extrapolation은 여전히 도전적 - 모델 예측과 실험 검증 간 괴리 해소 필요
- 향후 active learning과 결합하여 실험 데이터로 모델 지속 개선 폐쇄루프 구축
- ML 가이드 단백질 설계가 효소, 항체, 치료 단백질 개발에 광범위 적용

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
