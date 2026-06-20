# A microwell platform for high-throughput longitudinal phenotyping and selective retrieval of organoids

## Citation (NLM)
Sockell A, Wong W, Longwell S, Vu T, Karlsson K, Mokhtari D, Schaepe J, Lo YH, Cornelius V, Kuo C, Van Valen D, Curtis C, Fordyce PM. A microwell platform for high-throughput longitudinal phenotyping and selective retrieval of organoids. Cell Syst. 2023;14(9):764-776. doi: 10.1016/j.cels.2023.08.002

**DOI:** [https://doi.org/10.1016/j.cels.2023.08.002](https://doi.org/10.1016/j.cels.2023.08.002)

---

## Background
- 오가노이드는 질병 연구(특히 암)에 강력한 실험 모델이나, 기존 벌크 배양에서는 개별 오가노이드 성장 추적이 어려움
- 벌크 매트릭스의 국소 공간 변이로 인해 표현형 이질성이 세포 내인성 차이인지 미세환경 차이인지 구분 불가
- 단일 오가노이드 해상도로 고속 정량적 표현형 프로파일링 및 유전자형-표현형 매핑 플랫폼 필요
- 선택적 회수 메커니즘으로 관심 표현형 오가노이드의 분자 프로파일링 가능해야 함

## Key Experiment Methods
1. **마이크로웰 플랫폼**: 소프트 리소그래피로 PDMS 마이크로웰 디바이스 제작, 웰당 단일 오가노이드 포획, 벌크 매트릭스 대비 균일한 미세환경 제공
2. **종적 표현형 추적**: 시간 경과 이미징(수일~수주)으로 성장률(면적 증가율), 세포 이동(중심점 변위), 상피-기저 극성(lumen 형성) 등 다양한 표현형 특성 정량 측정
3. **선택적 오가노이드 회수**: 관심 표현형(예: 고속 성장, 특정 극성 패턴) 오가노이드를 마이크로웰에서 피펫으로 물리적으로 회수, 단일 오가노이드 DNA/RNA 추출 → 시퀀싱(WES, RNA-seq, ATAC-seq)
4. **딥러닝 이미지 분석 파이프라인**: U-Net 기반 오가노이드 세그멘테이션, 특징량 추출 자동화, 분석 스위트 통합으로 웰당 수백 개 오가노이드 동시 처리
5. **CRISPR 조작 인간 위 오가노이드 모델**: 종양 억제유전자(TP53, APC 등) KO 오가노이드로 유전적 변화와 표현형 연관성 검증

## Results
- 단일 세포/오가노이드 해상도로 고속 표현형 프로파일링 성공, 마이크로웰당 1개 오가노이드로 중첩 없이 종적 추적
- 성장률 증가와 관련된 유전체 변화 규명: 특정 돌연변이 조합이 성장 가속화와 연관, 단일 오가노이드 WES로 유전자형 확인
- 상피-기저 극성과 연관된 chromatin accessibility·유전자 발현 변화 규명: ATAC-seq으로 극성 관련 유전자 프로모터 접근성 변화 확인, RNA-seq으로 발현 프로파일 차이 확인
- 유전자형-표현형 매핑을 위한 단일 오가노이드 시퀀싱과 물리적 회수 메커니즘 통합, 같은 오가노이드에서 이미지 데이터 + 유전체 데이터 동시 획득
- 종적 추적으로 개별 오가노이드의 시간 경과 표현형 변화 정량화, 벌크 배양에서는 불가능했던 이질성 패턴 규명
- 마이크로웰 플랫폼이 organoid heterogeneity 연구와 맞춤형 약물 스크리닝에 유효함 입증

## Perspective
- 마이크로웰 플랫폼이 오가노이드 기반 고속 약물 스크리닝 및 질병 모델링에 기여
- 선택적 회수와 단일 오가노이드 시퀀싱 결합이 정밀 의학 연구에 유용
- 딥러닝 기반 이미지 분석이 오가노이드 표현형 분석의 표준 도구로 자리잡을 것
- 환자 유래 오가노이드 코호트에서 개인별 반응 예측으로 맞춤형 치료 가능
- 자동화 이미징과 마이크로웰 제어 결합이 오가노이드 연구 패러다임 변화

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
