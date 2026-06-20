# Integrated Micro-Devices for a Lab-in-Organoid Technology Platform: Current Status and Future Perspectives

## Citation (NLM)
Angotzi GN, Giantomasi L, Ribeiro JF, Crepaldi M, Vincenzi M, Zito D, Berdondini L. Integrated Micro-Devices for a Lab-in-Organoid Technology Platform: Current Status and Future Perspectives. Front Neurosci. 2022;16:842265. doi: 10.3389/fnins.2022.842265

**DOI:** [https://doi.org/10.3389/fnins.2022.842265](https://doi.org/10.3389/fnins.2022.842265)

---

## Overview

**Lab-in-Organoid (LIO)** 기술 개념을 소개하고 현황을 정리한 논문. 뇌 오가노이드 내부에 CMOS 기반 초소형 무선 마이크로디바이스를 삽입하여 세포 자가조립(self-aggregation) 과정에서 디바이스가 조직 내에 통합되도록 하는 접근이다. 기존 오가노이드 연구가 외부 전극이나 광학 기법에 의존하여 장기적·연속적 전기생리 측정에 한계가 있었던 문제를 해결하고자 한다. 이 논문은 이탈리아 IIT 그룹의 선행 연구 결과를 종합하고 근거리 무선 RF(Radio Frequency) 전력 전송 방식의 가능성을 실험적으로 검증한다.

---

## Key Topics

**뇌 오가노이드의 기존 측정 기술의 한계**
- 패치클램프: 단일 세포 고해상도이나 침습적·비연속적
- 칼슘 이미징: 수십~수백 세포 동시 측정 가능하나 공간/시간 해상도 제한
- MEA(다전극 배열): 표면 또는 관통형, 오가노이드 발달 전 기간(수개월) 연속 측정 불가

**Lab-in-Organoid 개념**
- 100×100 µm 크기의 CMOS 실리콘 마이크로디바이스를 세포 배양 중 혼합
- 표면 기능화(functionalization)로 세포 자가조립 시 디바이스가 구형체(spheroid) 내부에 포함
- 무선 근거리 RF(Near-field RF) 방식으로 전력 공급 및 데이터 전송
- 마이크로유체 채널을 통해 오가노이드를 하나씩 Base reader 앞에 통과시키며 리딩

**RF 무선 전송 실험 결과**
- 신경 구형체에 정현파 전자기장(RF 범위) 조사 시 신경세포 생존율, 세포 형태, 기능에 유의한 영향 없음 확인
- 비열적(non-thermal) 조건에서 RF 전자기장 노출이 세포에 안전함을 시사

**기존 시스템과의 비교**
- Li et al. (2019), McDonald et al. (2021) 등 선행 연구와 달리, 완전 무선·비삽관(untethered) 방식으로 더 높은 확장성 지향
- CMOS 온칩(on-chip) RF 구현으로 MEMS 후처리 없이 비용 절감 가능

---

## Key Findings

- 100 µm 급 CMOS 마이크로디바이스가 표면 기능화를 통해 신경 구형체 내부에 성공적으로 통합됨
- 무선 전력 전송에 필요한 수준의 RF 전자기장이 신경 구형체에 세포독성을 유발하지 않음
- LIO 플랫폼은 뇌 오가노이드의 장기적(수개월) 전기생리 연속 모니터링과 약물 반응성 functional assay 구현 가능성을 제시
- 근거리 RF는 초음파·광학 방식 대비 CMOS 온칩 구현이 용이하여 비용 효율적

---

## Perspective

LIO 기술이 성숙하면 뇌 발달 연구, 뇌 질환 모델링, 신약 스크리닝 등에서 기존 평면 배양이나 동물 모델을 대체할 수 있는 고충실도 in vitro 플랫폼이 될 수 있다. 향후 과제는 단일 디바이스에서 다채널 전극 어레이로의 확장, 실제 오가노이드(구형체 이상) 적용, 그리고 장기 배양 안정성 검증이다.

---

## Key References

- Lecomte A et al. (2020) Surface functionalization of silicon micro-devices for bio-artificial organoids. *Adv Mater Technol* [doi:10.1002/admt.202000789](https://doi.org/10.1002/admt.202000789)
- Li Q et al. (2019) Cyborg organoids: implantation of nanoelectronics via organogenesis for tissue-wide electrophysiology. *Nano Lett* 19(8):5781-5789. [doi:10.1021/acs.nanolett.9b02512](https://doi.org/10.1021/acs.nanolett.9b02512)
- Velasco S et al. (2019) Individual brain organoids reproducibly form cell diversity of the human cerebral cortex. *Nature* 570:523-527. [doi:10.1038/s41586-019-1289-x](https://doi.org/10.1038/s41586-019-1289-x)

---

*Processed by **Claude Sonnet 4.6** (Claude Code) on 2026-06-20*
