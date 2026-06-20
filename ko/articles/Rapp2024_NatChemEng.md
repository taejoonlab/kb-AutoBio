# Self-driving laboratories to autonomously navigate the protein fitness landscape

## Citation (NLM)
Rapp JT, Bremer BJ, Romero PA. Self-driving laboratories to autonomously navigate the protein fitness landscape. Nat Chem Eng. 2024;1:97-107. doi: 10.1038/s44286-023-00002-4

**DOI:** [https://doi.org/10.1038/s44286-023-00002-4](https://doi.org/10.1038/s44286-023-00002-4)

---

## Background
- 단백질 공학은 화학, 에너지, 의학 분야에서 광범위한 응용 가능성이 있으나, 새로운 기능의 단백질 창출은 느리고 노동집약적임
- 인간 연구자의 가설-실험-해석 사이클은 비효율적이며 수년 소요
- 로봇 과학자와 self-driving laboratory는 자동화된 학습·추론·실험으로 과학적 발견 가속화
- 생물학적 표현형은 복잡하고 비선형적이며, 유전체 탐색 공간은 고차원적이어서 자율 단백질 공학은 특히 어려움
- 기존 자동화 워크플로우는 일부 인간 개입이 필요하여 완전 자율적이지 않음

## Key Experiment Methods
1. **SAMPLE 플랫폼**: Self-driving Autonomous Machines for Protein Landscape Exploration - 지능형 에이전트가 단백질 서열-기능 관계를 학습하고 새 단백질 설계, Strateos Cloud Lab에 구현
2. **조합 서열 공간 설계**: DNA assembly graph로 GH1 조합 공간 정의, 자연계 GH1 + Rosetta 설계 + 진화정보 설계 fragment 조합, 총 1,352개 고유 GH1 서열(평균 116개 돌연변이, 최소 16개), TIM barrel fold 전반에 다양성 분포, 사이트당 최대 6개 아미노산 샘플링
3. **다중 출력 GP 모델**: 활성/비활성 분류와 연속적 특성(내열성 T50) 동시 예측, cytochrome P450 데이터 벤치마크(331 비활성+187 활성)에서 분류 정확도 83%, 활성 서열 내열성 예측 r=0.84
4. **베이지안 최적화 알고리즘**: UCB positive(Pactive>0.5만 고려), Expected UCB(Pactive×UCB 기댓값) - 비활성 '구멍' 회피, P450 시뮬레이션 10,000회 기준 median 26회 측정으로 최적 도달(표준 UCB median 83회, random median 108회)
5. **완전 자동화 실험 파이프라인**: Golden Gate 클로닝(유전자 조립, ~1h) → PCR(1h, EvaGreen dsDNA 검증) → T7 기반 cell-free 단백질 발현(3h) → 색도 분석 내열성 T50 측정(3h) = 총 9h/design-to-data
6. **예외 처리 및 데이터 품질 관리**: 3개 체크포인트(유전자 조립/PCR 성공, 반응 곡선 sigmoid 적합, 배경 활성 대비 측정), 실패 시 inconclusive 플래그 → 큐로 재투입, ~9% 실험 실패(액체 처리 오류)

## Results
- 4개 독립 SAMPLE 에이전트 배포, 각각 동일한 6개 자연 GH1 서열로 시드, Expected UCB 기준 매 라운드 3개 서열 선택, 총 20라운드 실행
- 모든 에이전트가 초기 서열보다 최소 12°C 더 안정한 효소 수렴(T50 기준), 전체 조합 공간의 <2%(약 60개/1,352개) 탐색
- 4개 에이전트 모두 동일한 global fitness peak로 수렴하지만 각 에이전트가 발견한 top 서열은 고유, thermostable 서열은 P6F0/P1F2/P5F2/P1F3 gene fragment 조합으로 구성
- 초기 탐색 단계에서 broad exploration, 후반 라운드에서 thermostable design 집중 샘플링
- 품질 필터가 2개 오류 데이터 놓침(Agent 1 round 10, Agent 3 round 5) - 의도적 미수정으로 에이전트 회복력 관찰, 추가 데이터 획득 후 정상 수렴
- inconclusive 실험 다수 발생(대부분 비활성 효소 2회 테스트 필요), 약 9% 실험 실패(액체 처리 오류)
- Expected UCB/UCB positive가 표준 UCB 대비 3-4배 적은 샘플로 최적 도달, 작은 배치 실행이 약간 유리

## Perspective
- self-driving laboratory가 단백질 공학 분야에서 완전 자율 design-test-learn 사이클 구현 가능함을 입증
- 베이지안 최적화와 자동화 실험의 통합이 단백질 최적화 효율을 획기적으로 개선
- SAMPLE 플랫폼은 범용 단백질 공학 플랫폼으로 다양한 생물공학·합성생물학 분야에 적용 가능
- 실험 측정 노이즈가 에이전트 탐색 행동에 영향을 주나, robust하게 수렴
- 향후 다중 목적 최적화, 더 큰 서열 공간, 복잡한 기능 특성으로 확장 가능

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
