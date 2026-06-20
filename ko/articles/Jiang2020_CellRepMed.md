# An Automated Organoid Platform with Inter-organoid Homogeneity and Inter-patient Heterogeneity

## Citation (NLM)
Jiang S, Zhao H, Zhang W, Wang J, Liu Y, Cao Y, Zheng H, Hu Z, Wang S, Zhu Y, Wang W, Cui S, Lobie PE, Huang L, Ma S. An automated organoid platform with inter-organoid homogeneity and inter-patient heterogeneity. Cell Rep Med. 2020;1(9):100161. doi: 10.1016/j.xcrm.2020.100161

**DOI:** [https://doi.org/10.1016/j.xcrm.2020.100161](https://doi.org/10.1016/j.xcrm.2020.100161)

---

## Background
- 기존 오가노이드 기술은 수동 조작으로 배치 간·오가노이드 간 변이가 크고, 4-6주 소요로 환자 맞춤형 약물 스크리닝에 시간적 제약
- 단일 세포 유래 오가노이드는 이질성 포획이 어렵고, 벌크 배양은 크기·세포 조성 불균일
- 종양 이질성을 포획하면서 모델 구축 기간을 단축하려면 1,000-2,000개 세포(통계적으로 종양 이질성 대표)를 정의된 Matrigel 부피에서 배양해야 함
- 고속·자동화 오가노이드 분배로 인건비·배치 간 변이 감소 필요

## Key Experiment Methods
1. **M1 모듈 (미세유체 기반 오가노이드 제작)**: 맞춤형 droplet-based 미세유체 시스템, 4°C 쿨러에서 Matrigel 용액 유지, PTFE 튜빙에서 cell-laden Matrigel droplet 생성(유상 HFE7000 + Matrigel 3-way PDMS connector), 37°C 수조에서 sol-gel 전이
2. **M2 모듈 (3D droplet 프린팅)**: 맞춤형 droplet printer로 XY motion stepwise 제어, 튜빙 outlet locomotion으로 개별 오가노이드 전구체를 96-well plate에 패턴링, HFE7000 휘발로 잔유물 없음
3. **최적화 파라미터**: 유량비(oil 30 µL/min, droplet 20 µL/min), 프린터 이동 속도(XY 500 mm/s, Z 20 mm/s), well당 standing time 2초, droplet 형성 주기와 XY motion 동기화
4. **단일 오가노이드 per well**: 95% 이상 성공률(96-well당 최대 4개 누락), 오가노이드 전구체 100-1,000개/10분 생성, 초당 1개 오가노이드 패턴링
5. **고속 개발**: droplet당 ~0.08 µL, ~1,506±13개 세포 포획(세포 밀도 2.0×10^7 cells/mL), 5-7일 만에 >400 µM 대형 오가노이드 달성(기존 4-6주 대비)

## Results
- 마우스 폐·간·신장 건강한 오가노이드와 인간 종양 오가노이드 모두 monodisperse 크기·분포, inter-organoid 변이 현저히 감소
- 건강한 오가노이드는 상피 조직 자가 조직화 재현, 종양 오가노이드는 상피 감소 패턴 - 부모 조직 특성 반영
- 조직학적 분석: 마이크로 스케일에서 부모 조직과 유사한 상피 조직 재현, 면역형광(E-cadherin, EpCAM)으로 상피 단층 도메인 확인
- 유전자 발현: 오가노이드가 부모 조직과 유사한 gene-expression profile, 종양 오가노이드가 부모 종양 유전자 돌연변이 97% 재현
- 21명 환자 조사에서 약물 반응 예측 정확도 >80%, 환자 간 변이(inter-patient heterogeneity) 명확히 반영
- 1주 만에 고속 약물 스크리닝 가능 - 환자 종양 샘플링부터 약물 평가·치료 추천까지 기간 단축

## Perspective
- 자동화 오가노이드 플랫폼이 맞춤형 암 치료 스크리닝의 timeliness 문제 해결
- inter-organoid homogeneity + inter-patient heterogeneity 동시 달성이 개인 맞춤형 의학 핵심
- 미세유체 + 3D 프린팅 융합이 오가노이드 제작·분배 패러다임 변화
- 향후 환자 유래 오가노이드 biobank 구축과 실시간 약물 반응 예측으로 정밀 의료 실현
- 자동화로 인건비 감소, 배치 간 변이 제거로 임상 적용 가능성 향상

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
