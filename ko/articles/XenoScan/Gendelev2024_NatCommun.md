# Deep phenotypic profiling of neuroactive drugs in larval zebrafish

## Citation (NLM)
Gendelev L, Taylor J, Myers-Turnbull D, Chen S, McCarroll MN, Arkin MR, Kokel D, Keiser MJ. Deep phenotypic profiling of neuroactive drugs in larval zebrafish. Nat Commun. 2024;15:9955. doi: 10.1038/s41467-024-54375-y

**DOI:** [https://doi.org/10.1038/s41467-024-54375-y](https://doi.org/10.1038/s41467-024-54375-y)

---

## Background
- CNS 약물 작용 기전은 GPCR·이온 채널 매개 경로의 복잡성과 polypharmacology로 인해 poorly understood
- Phenotypic screening이 단일 타겟 접근법의 한계를 우회하여 복잡한 생물학적 읽기값 우선시
- 유충 제브라피시는 고속 소분자 스크리닝 포맷으로 포유류 생리학 관련 신경활성 분자 발견에 활용
- 기존 correlation distance 기반 표현형 거리 계산이 미세 표현형 구분 실패, shortcut learning 문제 발생

## Key Experiment Methods
1. **고속 제브라피시 행동 스크리닝**: 96-well plate에서 650개 CNS 활성 화합물 고반복 스크리닝, 광/음향 자극으로 행동 반응 기록
2. **Motion Index(MI) 시계열**: 비디오 프레임에서 bulk motion 측정, 전통적으로 correlation distance로 표현형 거리 계산
3. **Deep metric learning 모델**: 제브라피시 행동 프로파일 학습, well-wise physical randomization으로 shortcut learning artifacts 제거
4. **Prospective in vitro 검증**: 인간 단백질 타겟 대상 radio-ligand binding assay로 모델 예측 검증(58% hit rate)
5. **최적화 파라미터**: well randomization 전략, MI time series 처리, metric learning 아키텍처, correlation distance vs learned distance 비교

## Results
- Deep metric learning 모델이 correlation distance 대비 표현형 거리 계산에서 월등한 성능
- Well-wise randomization으로 초기 모델의 shortcut learning(미세 실험 artifacts 활용) 문제 해결
- Orthogonal dataset(diverse drug-like compounds)로 일반화 능력 확인
- Prospective in vitro 검증에서 58% hit rate 달성, 종 간·화학 scaffold 경계 초월
- 제브라피시 표현형 스크리닝 + metric learning이 robust scaffold hopping capability 입증

## Perspective
- Deep metric learning이 고속 phenotypic screening 데이터 분석의 표준 도구로 자리잡을 것
- Well randomization이 phenotypic screening에서 shortcut learning 방지의 핵심
- 제브라피시 행동 스크리닝이 CNS 신약 발견·타겟 deconvolution에 광범위 적용
- 향후 다중 자극·다중 시간尺度 통합으로 표현형 해상도 향상
- 종 간 번역 가능성(translatability) 검증이 preclinical drug discovery 파이프라인 가속화

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
