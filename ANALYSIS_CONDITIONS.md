# PDF 분석 조건 기록

## 분석 일시
2026-06-20

## 분석 도구
- **PDF 텍스트 추출**: PyMuPDF (fitz), 최대 2-3페이지 텍스트 추출
- **DOI 메타데이터 조회**: CrossRef API (https://api.crossref.org/works/{doi})
  - User-Agent: `mailto:test@example.com`
  - 조회 항목: first author family name, published year, short container title (journal abbreviation)
- **파일명 정리**: `tools/process_pdf.py`로 DOI 추출 및 텍스트 생성, 파일명은 CrossRef 결과 기반으로 수동 검증 후 rename

## 논문 분류 기준

### 주제 범위 (Autonomous Lab / 실험자동화)
- **포함**: 자율 실험실(self-driving lab), 로봇 세포배양, 자동화 organoid/3D culture, AI 기반 실험 설계, 고속 phenotyping, 자동화 제조/manufacturing, laboratory automation, autonomous experimentation, automated liquid handling, biofoundry
- **제외**: 순수 단백질 설계/계산 이론, 순수 생물학/의학 연구(자동화·로봇공학과 무관), 일반적인 리뷰, EV 진단/액체 biopsy(자동화 플랫폼 아닌 분석 방법 논문)

### 분류 규칙
| 구분 | 파일명 규칙 | MD 노트 | 판단 기준 |
|------|-----------|---------|----------|
| 원저 연구 | `FirstAuthorYYYY_Journal.pdf` | 생성 (ko/en 쌍) | 실험자동화 관련 원저 |
| 리뷰 논문 | `FirstAuthorYYYY_Journal-review.pdf` | 생성하지 않음 | 제목/초록에 "review" 명시, 기존 문헌 종합 |
| off_topic | `원본파일명-off_topic.pdf` | 생성하지 않음 | 주제 범위 밖 (단백질 설계 순수 이론, 순수 생물학, EV 진단 등) |
| 중복 | `원본파일명-duplicate.pdf` | 생성하지 않음 | bioRxiv preprint, 동일 논문 duplicate |

## PDF 분류 결과 (ko/pdf/ 루트, 45개)
- **원저 연구**: 20개
- **리뷰**: 9개
- **off_topic**: 14개
- **중복**: 2개

## MD 노트 생성 규칙
- **형식**: 6개 섹션 (Title → Citation (NLM) → Background → Key Experiment Methods → Results → Perspective)
- **언어**: ko/en 쌍으로 생성 (bilingual mirror)
- **저장 위치**: `ko/articles/`, `en/articles/`
- **파일명**: `FirstAuthorYYYY_Journal.md`
- **Result 섹션**: 자동화 최적화 파라미터와 구체적 수치 포함
- **메타데이터**: 파일 하단에 `*Processed by **opencode** (opencode-go) on 2026-06-20*` 기록

## 생성된 MD 노트 (20개 논문, 40개 파일)
| 논문 | DOI |
|------|-----|
| Szymanski2023_Nature | 10.1038/s41586-023-06734-w |
| Rapp2024_NatChemEng | 10.1038/s44286-023-00002-4 |
| Hickman2023_Matter | 10.1016/j.matt.2023.02.007 |
| Adam2024_PNAS | 10.1073/pnas.2406320121 |
| Kanda2022_eLife | 10.7554/eLife.77007 |
| Tomasi2020_CellRep | 10.1016/j.celrep.2020.107670 |
| Imai2018_RegenTher | 10.1016/j.reth.2018.06.001 |
| Sockell2023_CellSyst | 10.1016/j.cels.2023.08.002 |
| Truong2021_SLASTechnol | 10.1177/2472630320972110 |
| Jiang2020_CellRepMed | 10.1016/j.xcrm.2020.100161 |
| Gustafson2021_LabChip | 10.1039/d0lc00940g |
| Ochs2021_Processes | 10.3390/pr9040575 |
| Archibald2016_BioprocessBiosystEng | 10.1007/s00449-016-1659-9 |
| Orsi2024_NatCommun | 10.1038/s41467-024-46574-4 |
| Koo2024_NatCommun | 10.1038/s41467-024-49123-1 |
| Freschlin2024_NatCommun | 10.1038/s41467-024-50712-3 |
| Qiu2021_NatComputSci | 10.1038/s43588-021-00168-y |
| DeBeuckeleer2025_eLife | 10.7554/eLife.95273 |
| Kane2019_SciRep | 10.1038/s41598-018-34828-3 |
| Tristan2021_StemCellRep | 10.1016/j.stemcr.2021.11.004 |
