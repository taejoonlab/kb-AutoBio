# Research Article Processing Skill

PDF 논문을 읽고 Obsidian용 MD 노트를 생성하는 스킬.

## When to Use

- 사용자가 새 PDF 논문을 vault에 추가하라고 요청할 때
- `ko/pdf/`에 새 PDF가 있고 MD 노트가 없을 때
- 기존 MD 노트를 업데이트하라고 요청할 때

## Workflow

### Step 0: PDF 분류 (리뷰 vs 원저)

PDF를 **리뷰 논문**과 **원저 연구**로 분류한다.

| 구분 | 파일명 접미사 | MD 노트 |
|------|-------------|---------|
| 원저 연구 | `(FirstAuthor)(Year)_(Journal).pdf` | 생성 |
| 리뷰 논문 | `(FirstAuthor)(Year)_(Journal)-review.pdf` | **생성하지 않음** |

**리뷰 판별 기준**: 제목·초록에 "review" 명시, "VIEWPOINT" 등 opinion 형식, 기존 문헌 종합·분석 논문

### Step 1: 파일명 확인

파일명 컨벤션: `FirstAuthorYYYY_Journal.pdf`

- `tools/process_pdf.py --dry-run`으로 제안된 이름 확인
- **자동 추출은 자주 실패**하므로 사람이 DOI로 직접 검증
- `ko/articles/`, `en/articles/`에 기존 파일과 충돌 없는지 확인

### Step 2: MD 노트 생성

**원저 연구 논문만** 대상으로 MD 노트를 생성한다. 리뷰 논문은 건너뛴다.

아래 형식으로 `ko/articles/FirstAuthorYYYY_Journal.md`와 `en/articles/FirstAuthorYYYY_Journal.md`를 **쌍으로** 생성:

```markdown
# 논문 제목

## Citation (NLM)
저자. 제목. 저널. 연도;권(호):쪽. doi:xxx

**DOI:** [URL](URL)

---

## Background
(연구 배경, 문제 제기)

---

## Key Experiment Methods
(주요 실험 방법, numbered list)

---

## Results
(주요 결과)

---

## Perspective
(의의, 한계, 향후 과제)

---

*Processed by **Qwen3.6 Plus** (opencode-go) on {YYYY-MM-DD}*
```

### Step 3: Commit

```bash
git add -A && git commit -m "add: ko FirstAuthorYYYY_Journal" && git push origin main
git add -A && git commit -m "add: en FirstAuthorYYYY_Journal" && git push origin main
```

## Rules

1. **절대 batch rename 하지 말 것** — 이름 충돌 시 silent overwrite 발생
2. **bilingual mirror 필수** — 원저 연구는 `ko/articles/`와 `en/articles/` 쌍으로 생성
3. **리뷰 논문은 MD 노트 생성 제외** — 파일명에 `-review` 접미사만 추가
4. **저자/저널은 DOI로 직접 검증** — `process_pdf.py` 자동 추출 신뢰하지 않음
5. **섹션 순서 엄수** — Title → Citation → Background → Key Experiment Methods → Results → Perspective → Processed by
6. **파일명 컨벤션** — `FirstAuthorYYYY_Journal.md` (e.g., `Wu2021_NatComm.md`)

## kb-AutoBio Project Rules

이 볼트는 **Autonomous Lab, 실험자동화** 관련 연구 논문을 다룬다. 아래 규칙을 엄수한다.

### 주제 범위

- **포함**: 자율 실험실(self-driving lab), 로봇 세포배양, 자동화 organoid/3D culture, AI 기반 실험 설계, 고속 phenotyping, 자동화 제조/manufacturing, laboratory automation, autonomous experimentation
- **제외**: 순수 생물학/의학 연구 중 자동화·로봇공학과 무관한 논문, 순수 이론/계산 연구, 일반적인 리뷰

### PDF 분류 규칙

| 구분 | 파일명 규칙 | MD 노트 |
|------|-----------|---------|
| 원저 연구 (관련) | `FirstAuthorYYYY_Journal.pdf` | 생성 (ko/en 쌍) |
| 리뷰 논문 | `FirstAuthorYYYY_Journal-review.pdf` | 생성하지 않음 |
| 주제 관련 없음 | `원본파일명-off_topic.pdf` | 생성하지 않음 |

### XenoScan 폴더

- `ko/pdf/XenoScan/` 하위 파일은 **폴더 구조를 그대로 유지**하며 처리
- `ko/articles/XenoScan/`, `en/articles/XenoScan/` 디렉토리에 대응 MD 생성
- 분류 규칙 동일 적용 (원저/review/off_topic)

## References

- 워크플로우 상세: `tools/SKILL.md`
- PDF 처리 스크립트: `tools/process_pdf.py`
