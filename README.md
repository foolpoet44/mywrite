

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
