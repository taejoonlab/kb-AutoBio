# Fully Automated Cultivation of Adipose-Derived Stem Cells in the StemCellDiscovery—A Robotic Laboratory for Small-Scale, High-Throughput Cell Production Including Deep Learning-Based Confluence Estimation

## Citation (NLM)
Ochs J, Biermann F, Piotrowski T, Erkens F, Nießing B, Herbst L, König N, Schmitt RH. Fully automated cultivation of adipose-derived stem cells in the StemCellDiscovery—a robotic laboratory for small-scale, high-throughput cell production including deep learning-based confluence estimation. Processes. 2021;9(4):575. doi: 10.3390/pr9040575

**DOI:** [https://doi.org/10.3390/pr9040575](https://doi.org/10.3390/pr9040575)

---

## Background
- 세포 기반 맞춤형 치료는 자동화가 전제되어야 비용 효율성과 광범위 접근성 달성 가능
- 환자 유래 세포 확장은 노동집약적이며 배치 간 변이가 큼, 개별 배치 크기는 작아 고속 처리 필요
- hMSC(인간 중간엽 줄기세포)는 지방·연골·골 세포로 분화 가능하며 조직 재생·면역 조절 기능
- 평면 배양이 소량 스크리닝에 적합하나, 자동화로 표준화·처리량·재현성 개선 필요

## Key Experiment Methods
1. **StemCellDiscovery 시스템**: Fraunhofer IPT 개발 완전 자동화 로봇 실험실, adherent 세포 병렬 배양, 지방 유래 hMSC 대상
2. **인라인 시각 품질 관리**: 고속 현미경 + 딥러닝 기반 이미지 처리로 자동 confluence 추정, 다양한 밀도에서 hMSC 검출 및 confluence 계산
3. **자동화 배양 워크플로우**: seeding → 배지 교환 → confluence 모니터링 → passaging 타이밍 결정 → 세포 확장, fully automated
4. **딥러닝 confluence 추정 알고리즘**: CNN 기반 세그멘테이션, 다양한 밀도 조건에서 학습, 수동 confluence 추정과 비교 검증
5. **생산 환경 시뮬레이션**: 시뮬레이션 소프트웨어로 StemCellDiscovery 용량 모델링, 고속 처리 조건에서 일일 처리 가능 plate 수 예측
6. **최적화 파라미터**: confluence 임계값(passaging trigger), 배지 교환 주기, seeding 밀도, passaging 비율, 로봇 처리 속도

## Results
- StemCellDiscovery가 지방 유래 hMSC 완전 자동화 확장 성공, confluence 추정 알고리즘으로 passaging 타이밍 자동 결정
- 딥러닝 confluence 추정 알고리즘이 다양한 세포 밀도에서 hMSC 검출 및 confluence 계산 성공
- 시뮬레이션 결과 로봇 실험실이 일일 95개 이상 cell culture plate 처리 가능
- 소량·고속 처리 조건에서 맞춤형 치료용 세포 생산 경제성 확보 가능성
- 자동화 배양이 수동 배양 대비 표준화·재현성·처리량 향상

## Perspective
- 완전 자동화 로봇 실험실이 세포치료제 소량·고속 생산의 핵심 인프라
- 딥러닝 기반 confluence 추정이 세포배양 품질 관리의 자동화 표준으로 발전 가능
- Industry 4.0과 바이오테크 융합이 맞춤형 치료 제조 패러다임 변화
- 향후 다중 세포 라인 동시 처리, 분화 프로토콜 자동화, 실시간 품질 모니터링으로 확장
- 자동화 생산 파이프라인이 세포치료제 상업화·보험 적용에 기여

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
