# AIEdu — Agentic AI로 돈 되는 웹앱 만들기

3일(1일 3시간 x 3일) 과정에서 만드는 "문의접수 웹앱" 저장소.

- 전체 설계는 [`PLAN.md`](./PLAN.md)를 따른다 — 작업을 시작하기 전에 반드시 먼저 읽는다.
- 교육 과정 슬라이드: https://docs.google.com/presentation/d/16tGynGPmL71UsK5N798315jIKfVT2I3hMxLz_uTlbS0/edit

## 에이전트 협업 방식

이 저장소는 두 에이전트가 역할을 분리해서 작업한다.

| | Claude Code | ChatGPT Codex |
|---|---|---|
| 역할 | 메인 작업 | GitHub 이슈 기반 위임 작업 |
| 작업 방식 | 로컬에서 실시간 pair-programming (지시 → 승인 → 실행) | GitHub 이슈를 읽고 PR로 작업을 올리는 비동기 작업 |
| 담당 | 진단·설계·구현·배포 전부 | PLAN.md에 명시된 2일차·3일차의 작은 위임 작업 2건만 |

Codex가 처음 이 저장소를 열면 [`AGENTS.md`](./AGENTS.md)를 먼저 읽는다.

## 진행 상태

- [x] 1일차-A: PLAN.md 초안 작성
- [ ] 1일차-B/C: 환경설정 + GitHub 연동 테스트 (학생 실습)
- [ ] 2일차: DB 연동 + AI 분류·요약 + 알림 + Codex 위임 1건
- [ ] 3일차: GCP/오라클 배포 + Codex 위임 2건째
