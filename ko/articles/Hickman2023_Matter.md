# Self-driving laboratories: A paradigm shift in nanomedicine development

## Citation (NLM)
Hickman RJ, Bannigan P, Bao Z, Aspuru-Guzik A, Allen C. Self-driving laboratories: A paradigm shift in nanomedicine development. Matter. 2023;6:1071-1081. doi: 10.1016/j.matt.2023.02.007

**DOI:** [https://doi.org/10.1016/j.matt.2023.02.007](https://doi.org/10.1016/j.matt.2023.02.007)

---

## Background
- 나노의약품은 mRNA-LNP 백신(코로나19) 등 임상적 성공을 거두었으나, 전임상 개발은 여전히 복잡하고 시간이 많이 소요됨
- 고차원 파라미터 공간(조성, 크기, 표면 특성 등)에서 최적 나노의약품 설계는 차원의 저주(curse of dimensionality)로 인해 전통적 실험 설계로는 비효율적
- Self-driving laboratory(SDL)는 자동화 실험 장비와 ML 기반 실험 계획을 결합하여 제한된 인간 개입으로 최적 후보 물질을 탐색
- 나노의약품 분야에 SDL 적용 사례는 아직 부족하며, 대규모 데이터셋 부재가 데이터 기반 방법의 한계

## Key Experiment Methods
1. **NanoMAP 제안**: Nanomedicine Materials Acceleration Platform - 고속실험(high-throughput experimentation) + AI(능동학습, few-shot 학습) + 데이터 공유 웹 애플리케이션 통합
2. **고속 실험**: 미세유체 기반 나노입자 합성으로 조성·공정 파라미터 공간 효율적 탐색, factorial design 대비 베이지안 최적화로 순차적 탐색
3. **ML 기반 실험 계획**: Gaussian process 기반 베이지안 최적화, acquisition function(UCB, EI 등)으로 exploration/exploitation 균형, 이전 실험 피드백 활용
4. **데이터 큐레이션**: 웹 기반 애플리케이션으로 나노의약품 특성(크기, zeta 전위, PDI, encapsulation efficiency)·성능 데이터 대규모 수집·공유, 데이터 표준화 포맷 제안
5. **Few-shot 학습**: 소량 데이터로도 일반화 가능한 전이학습, 메타러닝으로 새로운 나노입자 클래스 예측
6. **SDL 아키텍처**: 자동화 합성(미세유체/로봇 액체 처리) → 고속 특성분석(DLS, HPLC, cryo-EM) → ML 실험 계획 → 폐쇄루프

## Results
- NanoMAP 개념 제안 및 아키텍처 설계 (Perspective 논문)
- SDL 성공 사례 리뷰: 화학(연속 흐름 최적화, 촉매 발견), 재료과학(페로브스카이트 태양전지, 광전지), 생명과학(효소 설계, 유전자 회로 최적화)
- 나노의약품 SDL 적용 시 최적화 파라미터: LNP 조성(이온화 지질, helper 지질, 콜레스테롤, PEG-지질 비율), 미세유체 공정 파라미터(유량비, 총 유량, 채널 geometry), 특성분석 파라미터
- 데이터 부재가 주요 장벽 - 현재 공개 나노의약품 데이터셋은 소규모, 이질적 포맷
- LNP-mRNA 백신 개발 사례: 조성 최적화에 수백-수천 개 실험 소요, SDL로 탐색 공간 10-100배 효율화 가능

## Perspective
- NanoMAP과 같은 SDL 플랫폼이 나노의약품 전임상 개발 기간을 획기적으로 단축할 수 있음
- 대규모 데이터 큐레이션 이니셔티브가 선행되어야 AI 기반 설계 접근법 가능
- 제약과학 커뮤니티의 광범위한 참여와 데이터 공유 문화 정착 필요
- bench-to-bedside 번역 개선으로 생명을 위협하는 질환 환자들에게 혁신적 의약품 제공 가능
- 나노의약품 SDL은 조성 최적화 외에도 안정성, 독성, 생체분포 예측 등으로 확장 가능

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
