# Automated fluorescence quantification of extracellular vesicles collected from blood plasma using dielectrophoresis

## Citation (NLM)
Gustafson KT, Huynh KT, Heineck D, Bueno J, Modestino A, Kim S, Gower A, Armstrong R, Schutt CE, Ibsen SD. Automated fluorescence quantification of extracellular vesicles collected from blood plasma using dielectrophoresis. Lab Chip. 2021;21:1318-1332. doi: 10.1039/d0lc00940g

**DOI:** [https://doi.org/10.1039/d0lc00940g](https://doi.org/10.1039/d0lc00940g)

---

## Background
- 종양 유래 exosome 및 extracellular vesicles(EV)는 조기 암 검진을 위한 가치 있는 바이오마커이나, 작은 크기(50-150 nm)와 낮은 부유 밀도로 혈액에서 회복 어려움
- 기존 초원심분리·필터링 기반 방법은 시간 소모적·노동집약적
- DEP(dielectrophoresis) 기반 lab-on-a-chip이 혈장에서 EV 효율적 회수 가능
- 조기 암 환자에서 바이오마커 농도가 낮아 SNR(signal-to-noise ratio) 개선과 배경 잡음 분리 중요

## Key Experiment Methods
1. **DEP 칩**: 원형 전극 planar microarray, AC 전압 인가로 non-uniform electric field 생성, pDEP(positive DEP)로 EV를 전극 가장자리(high-field region)에 포집, hydrogel layer로 전극과 혈장 분리
2. **자동화 형광 정량 알고리즘(MATLAB)**: 전극 geometry 기반으로 ROI(collection region)와 BG(background region) 자동 식별, 국소 잡음 제거(평균+3σ), 광학 아티팩트 자동 제거
3. **내부 표준(internal standard)**: 알려진 농도의 형광 NP를 샘플에 spiking, DEP 칩 간 collection efficiency 변이 보정, 타겟 바이오마커와 동시 포집·정량
4. **최적화 파라미터**: AC 전압 주파수·진폭, 유량, 포집 시간, 형광 노출 시간, ROI/BG 영역 정의 임계값, 내부 표준 농도
5. **사용 가능 동적 범위**: 형광 강도 1-2000 a.u., 노출 시간·입자 농도에 대해 선형 증가

## Results
- 자동화 알고리즘이 수동 아티팩트 제거와 거의 동일한 성능(Pearson's r=0.999, 0.998, 36명 환자 2개 바이오마커)
- 사용 가능 동적 범위(1-2000 a.u.) 내에서 형광 강도가 노출 시간·입자 농도에 선형 비례
- 내부 표준 사용으로 DEP 칩 간 collection efficiency 변이 감소, 특히 저농도 바이오마커에서 효과적
- 내부 표준이 형광 강도-노출 시간 선형 추세 유지, 형광 강도-입자 농도 선형 추세 개선
- 조기 암 환자 혈장에서 낮은 SNR 환경에서도 바이오마커 정량 가능
- DEP 기반 EV 포집 + 자동화 형광 정량이 liquid biopsy 플랫폼으로 유효함 입증

## Perspective
- 자동화 형광 정량 알고리즘이 DEP 칩뿐 아니라 예측 가능한 포집 영역을 가진 lab-on-a-chip 전반에 적용 가능
- 내부 표준 접근법이 칩 간·실험 간 변이 보정의 표준 도구로 자리잡을 것
- 조기 암 검진을 위한 high-sensitivity liquid biopsy 플랫폼 발전에 기여
- 다중 바이오마커 동시 정량으로 암 특이성·민감도 향상 가능
- 임상 적용을 위한 표준화·검증 프로토콜 필요

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
