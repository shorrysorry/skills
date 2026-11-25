# skills

에이전트·라이브러리·오픈소스에서 발견한 유용한 skills 모음.

## 구조

```
dev/
  planning/       요구사항 정리, 설계, 구현 계획
  implementing/   계획 실행, 서브에이전트·병렬 작업
  testing/        TDD, 완료 전 검증
  debugging/      원인 추적
  review/         코드 리뷰 요청·수용
  git-workflow/   worktree, 브랜치 마무리
non-dev/    개발 외 작업 (글쓰기, 리서치, 생산성 등)
meta/       skill을 쓰거나 만들거나 관리하는 skills
_licenses/  출처별 원본 라이선스 전문
_templates/ 새 skill 추가용 템플릿
```

하위 카테고리는 skill이 5개쯤 쌓이면 실제 사용 패턴에 맞춰 나눈다 (최대 2단계).

## 새 skill 추가 방법

1. 주 용도에 맞는 카테고리 폴더 아래 `<skill-name>/` 생성
2. 원본 `SKILL.md`(와 딸린 파일)를 **수정 없이** 복사
3. `_templates/SOURCE.md`를 복사해 출처·라이선스·메모 작성
4. 아래 목록 표에 한 줄 추가

> 라이선스가 없는 원본은 복사하지 않고 `SOURCE.md`에 링크와 메모만 남긴다 (이 레포는 public).

## 목록

| Skill | 카테고리 | 용도 (한 줄) | 태그 | 출처 |
|---|---|---|---|---|
| [brainstorming](dev/planning/brainstorming/) | dev/planning | 기능·컴포넌트 등 창작 작업 전에 질문으로 요구사항과 설계를 먼저 다듬음 | planning | obra/superpowers |
| [writing-plans](dev/planning/writing-plans/) | dev/planning | 스펙을 코드 건드리기 전 단계별 구현 계획으로 분해 | planning | obra/superpowers |
| [dispatching-parallel-agents](dev/implementing/dispatching-parallel-agents/) | dev/implementing | 공유 상태 없는 2개 이상 작업을 병렬 에이전트로 분배 | subagent, parallel | obra/superpowers |
| [executing-plans](dev/implementing/executing-plans/) | dev/implementing | 작성된 계획을 현재 세션에서 직접 체크포인트 단위로 실행 | execution | obra/superpowers |
| [subagent-driven-development](dev/implementing/subagent-driven-development/) | dev/implementing | 계획의 독립 태스크를 서브에이전트에 맡기고 태스크마다 리뷰 | execution, subagent | obra/superpowers |
| [test-driven-development](dev/testing/test-driven-development/) | dev/testing | 구현 전에 실패하는 테스트부터 작성하는 Red→Green→Refactor | tdd | obra/superpowers |
| [verification-before-completion](dev/testing/verification-before-completion/) | dev/testing | 완료·통과 주장 전에 검증 명령을 실제로 돌리고 증거 확인 | verification | obra/superpowers |
| [systematic-debugging](dev/debugging/systematic-debugging/) | dev/debugging | 버그·테스트 실패 시 수정안 전에 근본 원인부터 체계적으로 추적 | debugging, root-cause | obra/superpowers |
| [receiving-code-review](dev/review/receiving-code-review/) | dev/review | 리뷰 피드백을 맹목 수용하지 않고 기술적으로 검증한 뒤 반영 | review | obra/superpowers |
| [requesting-code-review](dev/review/requesting-code-review/) | dev/review | 작업 완료·머지 전에 요구사항 충족 여부 리뷰 요청 | review | obra/superpowers |
| [finishing-a-development-branch](dev/git-workflow/finishing-a-development-branch/) | dev/git-workflow | 구현 완료 후 머지/PR/정리 등 통합 방식 결정 | git, merge, pr | obra/superpowers |
| [using-git-worktrees](dev/git-workflow/using-git-worktrees/) | dev/git-workflow | 기능 작업을 격리된 git worktree에서 시작 | git, worktree | obra/superpowers |
| [diagnosing-superpowers](meta/diagnosing-superpowers/) | meta | superpowers 세션이 잘못 흘러간 원인을 사후 진단 | retrospective | obra/superpowers |
| [using-superpowers](meta/using-superpowers/) | meta | 대화 시작 시 skill을 찾아 먼저 호출하도록 하는 사용 규칙 | skill-usage | obra/superpowers |
| [writing-skills](meta/writing-skills/) | meta | 새 skill 작성·수정과 배포 전 동작 검증 | skill-authoring | obra/superpowers |
