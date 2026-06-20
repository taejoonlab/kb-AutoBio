# EmbryoNet: using deep learning to link embryonic phenotypes to signaling pathways

## Citation (NLM)
Čapek D, Safroshkin M, Morales-Navarrete H, Toulany N, Arutyunov G, Kurzbach A, Bihler J, Hagauer J, Kick S, Jones F, Jordan B, Müller P. EmbryoNet: using deep learning to link embryonic phenotypes to signaling pathways. Nat Methods. 2023;20:815-823. doi: 10.1038/s41592-023-01873-4

**DOI:** [https://doi.org/10.1038/s41592-023-01873-4](https://doi.org/10.1038/s41592-023-01873-4)

---

## Background
- 초기 발생은 BMP, RA, Wnt, FGF, Nodal, Shh, PCP 등 7개 주요 신호전달 경로에 의해 조절되며, 이들 경로의 기능 상실은 특징적인 발생 결함을 유발
- 표현형 결함 분류는 근본적인 신호전달 기전을 식별할 수 있으나 전문가 지식에 의존하고 분류 체계가 표준화되지 않음
- 제브라피시 발생 이미지의 고속·정량적 표현형 분석을 위한 자동화 플랫폼 필요

## Key Experiment Methods
1. **EmbryoNet 딥러닝 모델**: ResNet 기반 합성곱 신경망(CNN)으로 제브라피시 신호전달 돌연변이체 자동 분류, 200만 장 이상 이미지 학습
2. **시간 의존적 발생 궤적 모델**: 발생 단계별(timestamp) 표현형 변화를 고려한 다중 타임스탬프 입력 아키텍처
3. **7개 신호전달 경로 분류**: BMP, RA, Wnt, FGF, Nodal, Shh, PCP 기능 상실 돌연변이체를 unbiased manner로 식별
4. **고속 약물 스크리닝 적용**: EmbryoNet을 high-throughput drug screen에 적용하여 화합물의 작용 기전(MOA) 규명
5. **최적화 파라미터**: CNN 레이어 구성(7×7, 3×3, 1×1 ConvRelu), residual block, global average pooling, timestamp channel 수, 학습 데이터 크기

## Results
- EmbryoNet이 제브라피시 7개 주요 신호전달 경로 돌연변이체를 고정밀도로 분류
- 시간 의존적 발생 궤적 모델과 결합하여 표현형 결함을 높은 정밀도로 식별·분류
- 진화적으로 먼 종에서도 신호전달 결함을 robust하게 식별
- 고속 약물 스크리닝에서 EmbryoNet이 약리학적 물질의 작용 기전을 분해능 있게 규명
- 200만 장 이상의 학습/테스트 이미지 공개

## Perspective
- 딥러닝 기반 자동 표현형 분석이 발생생물학 및 신호전달 경로 연구에 광범위하게 적용 가능
- 고속 약물 스크리닝과 결합하여 신약 개발의 MOA 규명 가속화
- 표준화된 분류 체계가 전문가 의존적 표현형 평가의 한계 해소
- 향후 다중 종·다중 발생 단계로 확장 가능한 범용 phenotyping 프레임워크
- 공개된 대규모 이미지 데이터셋이 발생 딥러닝 연구의 기반 인프라로 기여

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
