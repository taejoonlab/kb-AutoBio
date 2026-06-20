# Robotic search for optimal cell culture in regenerative medicine

## Citation (NLM)
Kanda GN, Tsuzuki T, Terada M, Sakai N, Motozawa N, Masuda T, Nishida M, Watanabe CT, Higashi T, Horiguchi SA, Kudo T, Kamei M, Sunagawa GA, Matsukuma K, Sakurada T, Ozawa Y, Takahashi M, Takahashi K, Natsume T. Robotic search for optimal cell culture in regenerative medicine. eLife. 2022;11:e77007. doi: 10.7554/eLife.77007

**DOI:** [https://doi.org/10.7554/eLife.77007](https://doi.org/10.7554/eLife.77007)

---

## Background
- 재생의학에서 유도 분화는 경험과 기술에 크게 의존하는 실험 과정이며, 최적 조건 확립에 수년 소요
- 세포배양은 화학적 자극(시약 종류·용량·타이밍)과 물리적 조작(피펫팅 강도, 진동, CO2 incubator 이동 등)이 결과에 큰 영향
- 기존 자동화 세포배양 장치는 고정 공정 자동화로, 유연한 파라미터 탐색에 한계
- 로봇 암은 인간과 달리 동일 작업을 고정밀도로 반복 가능하며, 모든 물리적 파라미터를 일정하게 유지하고 오류 로깅 가능

## Key Experiment Methods
1. **LabDroid 시스템**: 범용 humanoid 로봇(Maholo)으로 세포배양 프로토콜 실행, dual arm 로봇, CO2 incubator, micro pipettes, microscope 통합, 내장 현미경으로 AI 기반 이미지 처리 및 세포 품질 평가
2. **iPSC-RPE 분화 프로토콜 디지털화**: seeding(DDay -7), preconditioning(DDay -6~-1), passage(DDay 0), RPE differentiation/induction(DDay 1~25), RPE maintenance culture(DDay 26~34)의 5단계, 8개 6-well plate 동시 처리(48 wells/batch)
3. **7개 최적화 파라미터 (약 2억 개 조합 공간)**:
   - PC (Preconditioning concentration): FGFRi 농도 0-505 nM
   - PP (Preconditioning period): FGFRi 처리 기간 1-6일
   - DP (Detachment trypsin period): 37°C 20분 후 실온 incubation 시간 5/8/11/14/17/20/23분 (contextual parameter, well마다 3분 간격 고정)
   - DS (Detachment pipetting strength): 피펫팅 강도 10-100 mm/s
   - DL (Detachment pipetting length): 피펫팅 바닥면적 short/long
   - KP (KSR period): KSR 농도 감소 기간 1-19일(매일 선형 감소, DDay KP에 10% 도달)
   - 3P (Three supplements period): Y-27632/SB431542/CKI-7 처리 기간 3-19일
4. **Batch Bayesian Optimization(BBO)**: GP posterior로 surrogate 모델 업데이트, acquisition function으로 다음 48개 파라미터 생성, BCLP(Batch Contextual Local Penalization) policy로 batch 내 중복 탐색 방지, trypsin 처리 시간(DP) context 매 라운드 조정
5. **품질 평가**: DDay 34 착색 면적 비율(pigmentation score)을 목적 함수, 이미지 처리로 자동 계산

## Results
- Baseline 실험(수동 프로토콜 단순 이식)에서 trypsin 37°C 20분 + 실온 14분 조건 최고 점수 0.44±0.03, 23분 조건 최저 0.33±0.02 - 물리적 파라미터(트립신 시간, 피펫팅 강도 등)가 분화 효율에 큰 영향
- 3라운드 BBO 최적화(111일, 143개 조건 탐색)로 baseline 대비 88% 향상된 iPSC-RPE 생산 달성
- 최적화 결과: FGFRi 저농도(0-50 nM) + 단기간(1-2일) preconditioning, trypsin 처리 시간 단축(8-14분), 약한 피펫팅 강도(10-30 mm/s), KSR 빠른 감소(KP 5-7일), 3보충제 단기간(3-7일)이 높은 착색 점수와 연관
- BBO 1라운드에서 급격한 점수 상승, 2-3라운드에서 수렴 - exploration에서 exploitation으로 전환
- 로봇이 생산한 iPSC-RPE 세포가 재생의학 연구 적용 기준 충족(형태학적 특징, 유전자 발현 프로파일, 이식 후 기능 확인)
- LabDroid가 48개 well 모두에서 착색 세포 검출, 운영 프로세스 오류 없음 - 높은 재현성과 오류 로깅으로 실험 투명성 확보

## Perspective
- 자율 로봇 AI 시스템이 세포배양 조건 탐색을 획기적으로 가속화할 수 있음 입증
- 재생의학뿐 아니라 약물 스크리닝, 조직 공학 등 다양한 분야에 적용 가능
- 로봇화와 AI 최적화의 결합이 실험실 자동화의 새로운 패러다임 제시
- 향후 다중 목적 최적화(착색+형태+유전자 발현 등)로 확장 가능
- LabDroid와 같은 범용 로봇이 연구실 프로토콜 변화에 유연하게 대응 가능

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
