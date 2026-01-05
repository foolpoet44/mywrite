
mywrite — Obsidian 기반 Mind Repository 

사고의 진화를 Markdown + GitHub로 관리하는 간소화된 워크플로 

 

📚 개요 

mywrite는 Obsidian Vault를 중심으로 아이디어를 기록 → 구조화 → 버전 관리 → 발행하는 프로세스를 제공합니다. 

Google 도구는 제거하고, Markdown 중심으로 단순화했습니다. 

 

🗂 폴더 구조 

1     mywrite/ 

2     ├─ inbox/        # 아이디어 캡처 

3     ├─ drafts/       # 초안 작성 

4     ├─ published/    # 최종 발행 

5     └─ Progress-Log.md # 주간 회고 

6      

 

🚀 워크플로 

1. Capture 

Obsidian Vault의 inbox/에 Markdown 파일 생성 

파일명: YYYYMMDD-topic.md 

2. Synthesize 

Obsidian에서 초안 작성 

Templater로 템플릿 자동 삽입 

Dataview로 상태별 문서 관리 

3. Commit 

Vault를 Git 저장소로 설정 

Obsidian Git 플러그인: 

Auto Commit: 30분 

Auto Push: 30분 

메시지: update({{fileName}}): status={{status}} 

4. Merge & Evolve 

GitHub Pull Request → 리뷰 → 머지 

머지 후: 

drafts/ → published/ 이동 

Progress-Log.md 업데이트 (자동화 가능) 

 

✅ 템플릿 예시 

--- 

title: "{{title}}" 

date: {{date}} 

status: draft 

tags: [insight] 

--- 

## 핵심 요지 

- 요지 1 

- 요지 2 

## 본문 

(내용 작성) 

## 다음 액션 

- [ ] 추가 자료 조사 

 

🔧 자동화 

Obsidian Git 플러그인으로 자동 커밋/푸시 

GitHub Actions: 

머지 시 published 폴더 이동 

Progress-Log.md 업데이트 

 

🤝 기여 

Issue: 아이디어 제안 

PR: 초안 리뷰 및 발행 승인 

 

📄 라이선스 

MIT 또는 CC-BY-4.0 권장 
