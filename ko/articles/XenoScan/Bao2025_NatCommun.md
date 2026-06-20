# Deep learning-based high-resolution time inference for deciphering dynamic gene regulation from fixed embryos

## Citation (NLM)
Bao H, Zhang S, Yu Z, Xu H. Deep learning-based high-resolution time inference for deciphering dynamic gene regulation from fixed embryos. Nat Commun. 2025;16:6565. doi: 10.1038/s41467-025-61907-7

**DOI:** [https://doi.org/10.1038/s41467-025-61907-7](https://doi.org/10.1038/s41467-025-61907-7)

---

## Background
- 배아 발생은 복잡한 유전자 조절 네트워크의 시공간적 동역학에 의해 주도, 전통적 live-imaging은 동시 분자 종 추적 제한(<4개)
- Fixed-embryo imaging이 높은 민감도·공간 해상도 제공하나 시간 분해능 부재
- 수동 staging 또는 morphology atlas 비교가 coarse-grained 단계만 제공, 분자 수준 동역학 해석 불가
- Deep learning으로 fixed embryo 이미지에서 핵 형태 기반 절대 발생 시간 고정밀 추론 필요

## Key Experiment Methods
1. **Multi-scale ensemble deep learning**: Drosophila fixed embryo 이미지에서 핵 형태 기반 절대 발생 시간 1분 해상도로 추론
2. **Fixed-embody quantitative imaging**: Wild-type 배아 고정·이미징으로 segmentation gene Krüppel(Kr)의 다중 전사인자(TF) 조절 해석
3. **Time-resolved theoretical model**: 단일 분자 mRNA 통계 모델과 통합, endogenous segmentation gene hunchback(hb)의 unsteady-state bursty kinetics 규명
4. **유전자 변형 없이 동역학 해석**: genetic modification 없이 endogenous gene regulation 동역학 규명
5. **최적화 파라미터**: multi-scale CNN 아키텍처, nuclear morphology 특징, time bin 크기, ensemble 구성, mRNA burst kinetics 모델 파라미터

## Results
- Deep learning이 fixed embryo 이미지에서 1분 해상도 절대 발생 시간 정확히 추론
- Segmentation gene Krüppel(Kr)의 다중 TF에 의한 시공간 조절 해석
- Hunchback(hb) 유전자의 unsteady-state bursty kinetics 동적 TF 결합에 의해 구동됨 규명
- Genetic modification 없이 complex gene network 동역학 해석 가능한 versatile 프레임워크 제공
- Fixed-embryo imaging의 시간 분해능 한계 딥러닝으로 극복

## Perspective
- Deep learning 기반 시간 추론이 발생 유전체학의 표준 분석 도구로 발전
- Fixed-embryo imaging + AI가 live-imaging 한계 우회, 다중 분자 종 동시 분석 가능
- Time-resolved 모델이 유전자 발현 burst kinetics 이해에 기여
- 다른 모델 생물(Drosophilla → 제브라피시, Xenopus, mammalian)로 확장 가능
- 발생 중 유전자 조절 네트워크 전체 지도 작성에 기여

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
