

# mywrite 🧠 — Mind Repository
> 사고의 버전 관리(Version Control of Thoughts)로 영감을 축적·정제·진화시키는 **창의적 글쓰기 스튜디오**

“기록되지 않은 생각은 존재하지 않는 소프트웨어와 같다.”

---

## 📚 개요 (Overview)
**mywrite**는 Google 생태계의 기동성과 GitHub의 체계성을 결합해, 파편화된 영감을 **수집→구조화→발행**하는 전 과정을 버전 관리합니다.  
핵심 워크플로: **Capture (Google Keep) → Synthesize (Gemini + Google Docs) → Commit (GitHub) → Merge & Evolve (PR 리뷰/병합)**

---

## 🗂 폴더 구조 (Directory Structure)
아래 구조는 저장소의 기본 원칙입니다. 최초 실행 시
mywrite/
├─ inbox/            # 날것의 아이디어/메모(.md) 수집 (Capture)
├─ drafts/           # 주제/형식별 초안 정리 (Refine)
├─ published/        # 퇴고 완료된 최종 원고 (Persist)
├─ assets/           # 이미지, 도표, 참고 PDF 등 보조 자산 (Support)
└─ Progress-Log.md   # 주별 변화/회고/피드백 로그 (Evolution)

### 📌 네이밍 규칙
- 파일: `YYYYMMDD-topic.md` (예: `20260105-agent-ethics.md`)
- 이미지: `topic-slug-001.png` (연번 관리)
- 라벨(태그): `#insight`, `#todo`, `#review`, `#publish-ready` 등 메타 태그를 문서 상단에 명시

---

## 🚀 시작하기 (Getting Started)

### 1) 초기 세팅
```bash
# 폴더 생성
mkdir -p inbox drafts published assets

# 회고 로그 파일 생성
touch Progress-Log.md

# (선택) 초기 커밋
git add .
git commit -m "chore: bootstrap mind repository structure"
git push -u origin main

2) 캡처 & 확장

Capture: 이동 중 떠오른 생각을 Google Keep에 기록
Synthesize: Gemini와 대화하며 아이디어 확장 → Google Docs에서 구조화
Convert: Docs를 Markdown으로 변환(예: Docs to Markdown 부가 기능) 후 inbox/ 또는 drafts/에 저장
Commit: 변화 맥락을 담은 커밋 메시지로 저장 (예: feat(drafts): add argument on agent ethics (#insight))


✍️ 문서 템플릿 (Markdown Template)
---
title: "에이전트 윤리: 도구인가, 행위자인가"
date: 2026-01-05
labels: ["insight", "ethics", "ai"]
status: "draft"       # draft | review | publish-ready | published
links:
  - ref: "논문/기사 링크"
  - ref: "관련 토론 스레드"
---

## 핵심 요지
- 요지 1
- 요지 2

## 본문
(핵심 주장, 논거, 반례, 사례, 시사점)

## 다음 액션
- [ ] 추가 자료 조사
- [ ] 반론 섹션 보강
- [ ] 도표/이미지 추가

🧭 워크플로 (Workflow)
Capture → Synthesize → Commit → Merge & Evolve

Small Commits: 작은 단위로 자주 커밋해 사고의 변화 경로를 남깁니다.
Meaningful Messages: “왜 바뀌었는지” 맥락을 담아 커밋을 기록합니다.
Branching Thoughts: 상이한 관점/구성은 브랜치로 실험합니다.


# 기능/관점 브랜치 생성
git checkout -b feature/agent-ethics-alt-view

# 편집/추가 후 커밋
git add drafts/20260105-agent-ethics.md
git commit -m "feat(drafts): add counter-argument on agent moral status"

# 원격 푸시 & PR 생성
git push -u origin feature/agent-ethics-alt-view
# GitHub에서 Compare & Pull Request → 자기 리뷰 → 코멘트 반영 → Merge
``







