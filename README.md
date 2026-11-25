# skills

에이전트·라이브러리·오픈소스에서 발견한 유용한 skills 모음.

## 구조

```
dev/
  planning/       요구사항 정리, 설계, 스펙, 구현 계획, 티켓 분해
  frontend/       React·Next.js·TypeScript 작성 패턴
  libraries/      특정 라이브러리 (Zustand, RHF, Storybook, shadcn, TanStack)
  ui-design/      UI 디자인 방향, 디자인 시스템, UI 리뷰
  implementing/   계획 실행, 서브에이전트·병렬 작업, 리뷰 요청
  testing/        TDD, 단위·E2E 테스트, 완료 전 검증
  debugging/      원인 추적
  review/         코드 리뷰, 단순화
  performance/    React·Next.js·앱 단위 성능 최적화
  web-quality/    Lighthouse 기준 성능·CWV·접근성·SEO·모범 사례 감사 (한 묶음)
  accessibility/  WCAG 접근성 구현·수정
  architecture/   모듈 구조·코드베이스 아키텍처
  git-workflow/   worktree, 브랜치 마무리
non-dev/
  visualization/  다이어그램, 차트 등 시각 산출물
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
| [spec-driven-development](dev/planning/spec-driven-development/) | dev/planning | 코딩 전에 스펙(PRD)을 먼저 작성 | spec, prd | addyosmani/agent-skills |
| [to-spec](dev/planning/to-spec/) | dev/planning | 지금까지의 대화를 스펙으로 정리해 이슈 트래커에 등록 | spec | mattpocock/skills |
| [to-tickets](dev/planning/to-tickets/) | dev/planning | 계획·스펙을 선후관계가 명시된 tracer-bullet 티켓으로 분해 | tickets | mattpocock/skills |
| [writing-plans](dev/planning/writing-plans/) | dev/planning | 스펙을 코드 건드리기 전 단계별 구현 계획으로 분해 | planning | obra/superpowers |
| [clean-code-ts-react](dev/frontend/clean-code-ts-react/) | dev/frontend | TS·React 코드의 네이밍·컴포넌트 형태·에러 처리 등 코드 품질 기준 | typescript, react, clean-code | pproenca/dot-skills |
| [composition-patterns](dev/frontend/composition-patterns/) | dev/frontend | boolean prop 남발을 줄이는 확장 가능한 React 컴포넌트 합성 패턴 | react, components | vercel-labs/agent-skills |
| [frontend-ui-engineering](dev/frontend/frontend-ui-engineering/) | dev/frontend | 접근성·반응형을 갖춘 프로덕션 수준 UI·컴포넌트 구현 | ui, components | addyosmani/agent-skills |
| [nextjs-app-router-patterns](dev/frontend/nextjs-app-router-patterns/) | dev/frontend | Next.js 14+ App Router의 Server Components·스트리밍·데이터 페칭 패턴 | nextjs, app-router | wshobson/agents |
| [react-best-practices](dev/frontend/react-best-practices/) | dev/frontend | Vercel의 React·Next.js 성능 규칙으로 코드 작성·리뷰·리팩토링 | react, nextjs, performance | vercel-labs/agent-skills |
| [react-modernization](dev/frontend/react-modernization/) | dev/frontend | React 버전 업그레이드, 클래스 컴포넌트→hooks, concurrent 기능 도입 | react, migration | wshobson/agents |
| [react-state-management](dev/frontend/react-state-management/) | dev/frontend | Redux Toolkit·Zustand·Jotai·React Query 중 상태 관리 방식 선택과 구성 | react, state | wshobson/agents |
| [react-view-transitions](dev/frontend/react-view-transitions/) | dev/frontend | React View Transition API로 네이티브 같은 화면 전환 애니메이션 구현 | react, animation | vercel-labs/agent-skills |
| [typescript-advanced-types](dev/frontend/typescript-advanced-types/) | dev/frontend | generics·conditional·mapped type 등 고급 타입으로 타입 안전한 코드 작성 | typescript, types | wshobson/agents |
| [react-hook-form](dev/libraries/react-hook-form/) | dev/libraries | React Hook Form 폼 검증과 리렌더 성능 최적화 | forms | pproenca/dot-skills |
| [shadcn](dev/libraries/shadcn/) | dev/libraries | shadcn/ui 공식: 컴포넌트 추가·검색·수정·스타일링과 프로젝트 관리 | shadcn, ui | shadcn-ui/ui |
| [storybook](dev/libraries/storybook/) | dev/libraries | Storybook 설정, CSF3 스토리 작성, 컴포넌트 라이브러리 문서화 | storybook | pproenca/dot-skills |
| [tanstack-integration](dev/libraries/tanstack-integration/) | dev/libraries | TanStack Query와 Router·Start 연동 시 데이터 흐름·SSR·캐시 조율 | tanstack | DeckardGer/tanstack-agent-skills |
| [tanstack-query](dev/libraries/tanstack-query/) | dev/libraries | TanStack Query 데이터 페칭·캐싱·mutation 모범 사례 | tanstack, data-fetching | DeckardGer/tanstack-agent-skills |
| [tanstack-router](dev/libraries/tanstack-router/) | dev/libraries | TanStack Router 타입 안전 라우팅·데이터 로딩·search params | tanstack, routing | DeckardGer/tanstack-agent-skills |
| [tanstack-start](dev/libraries/tanstack-start/) | dev/libraries | TanStack Start 서버 함수·미들웨어·SSR·인증 패턴 | tanstack, fullstack | DeckardGer/tanstack-agent-skills |
| [zustand](dev/libraries/zustand/) | dev/libraries | Zustand 스토어 작성·리뷰 시 성능과 구조 모범 사례 | zustand, state | pproenca/dot-skills |
| [design-system-patterns](dev/ui-design/design-system-patterns/) | dev/ui-design | 디자인 토큰·테마·컴포넌트 아키텍처로 디자인 시스템 구축 | design-system, tokens | wshobson/agents |
| [frontend-design](dev/ui-design/frontend-design/) | dev/ui-design | 새 UI를 만들 때 뻔하지 않은 미적 방향·타이포그래피·레이아웃 결정 | design | anthropics/skills |
| [web-artifacts-builder](dev/ui-design/web-artifacts-builder/) | dev/ui-design | React·Tailwind·shadcn으로 다중 컴포넌트 HTML artifact 제작 | react, tailwind, artifact | anthropics/skills |
| [web-design-guidelines](dev/ui-design/web-design-guidelines/) | dev/ui-design | Web Interface Guidelines 기준으로 UI 코드 리뷰 (디자인·접근성·UX) | ui-review, a11y | vercel-labs/agent-skills |
| [dispatching-parallel-agents](dev/implementing/dispatching-parallel-agents/) | dev/implementing | 공유 상태 없는 2개 이상 작업을 병렬 에이전트로 분배 | subagent, parallel | obra/superpowers |
| [executing-plans](dev/implementing/executing-plans/) | dev/implementing | 작성된 계획을 현재 세션에서 직접 체크포인트 단위로 실행 | execution | obra/superpowers |
| [requesting-code-review](dev/implementing/requesting-code-review/) | dev/implementing | 작업 완료·머지 전에 요구사항 충족 여부 리뷰 요청 | review | obra/superpowers |
| [subagent-driven-development](dev/implementing/subagent-driven-development/) | dev/implementing | 계획의 독립 태스크를 서브에이전트에 맡기고 태스크마다 리뷰 | execution, subagent | obra/superpowers |
| [browser-testing-with-devtools](dev/testing/browser-testing-with-devtools/) | dev/testing | Chrome DevTools MCP로 실제 브라우저에서 DOM·콘솔·네트워크 확인 | devtools, browser | addyosmani/agent-skills |
| [e2e-testing-patterns](dev/testing/e2e-testing-patterns/) | dev/testing | Playwright·Cypress로 안정적인 E2E 테스트 스위트 구축 | playwright, cypress | wshobson/agents |
| [javascript-testing-patterns](dev/testing/javascript-testing-patterns/) | dev/testing | Jest·Vitest·Testing Library로 단위·통합·E2E 테스트 전략과 mock | jest, vitest, rtl | wshobson/agents |
| [playwright-skill](dev/testing/playwright-skill/) | dev/testing | 최신 Playwright 패턴 묶음 (core·POM·CI·frontend·마이그레이션·QA) | playwright, e2e, ci, pom | testdino-hq/playwright-skill |
| [react-testing-library](dev/testing/react-testing-library/) | dev/testing | 사용자 관점의 유지보수 쉬운 React Testing Library 테스트 작성 | rtl | pproenca/dot-skills |
| [tdd](dev/testing/tdd/) | dev/testing | red-green-refactor로 기능 구현·버그 수정을 테스트부터 진행 | tdd | mattpocock/skills |
| [test-driven-development](dev/testing/test-driven-development/) | dev/testing | 구현 전에 실패하는 테스트부터 작성하는 Red→Green→Refactor | tdd | obra/superpowers |
| [verification-before-completion](dev/testing/verification-before-completion/) | dev/testing | 완료·통과 주장 전에 검증 명령을 실제로 돌리고 증거 확인 | verification | obra/superpowers |
| [vitest](dev/testing/vitest/) | dev/testing | Vitest 설정·비동기 테스트·vi mock·스냅샷·테스트 성능 패턴 | vitest | pproenca/dot-skills |
| [webapp-testing](dev/testing/webapp-testing/) | dev/testing | Playwright로 로컬 웹앱 기능 검증·UI 디버깅·스크린샷 | playwright, e2e | anthropics/skills |
| [diagnosing-bugs](dev/debugging/diagnosing-bugs/) | dev/debugging | 어려운 버그·성능 회귀를 진단 루프로 추적 | debugging, regression | mattpocock/skills |
| [systematic-debugging](dev/debugging/systematic-debugging/) | dev/debugging | 버그·테스트 실패 시 수정안 전에 근본 원인부터 체계적으로 추적 | debugging, root-cause | obra/superpowers |
| [code-review](dev/review/code-review/) | dev/review | 기준 커밋 이후 변경을 레포 컨벤션 준수·정확성 두 축으로 리뷰 | review | mattpocock/skills |
| [code-simplification](dev/review/code-simplification/) | dev/review | 동작은 유지한 채 읽기 어려운 코드를 단순화 | refactor | addyosmani/agent-skills |
| [receiving-code-review](dev/review/receiving-code-review/) | dev/review | 리뷰 피드백을 맹목 수용하지 않고 기술적으로 검증한 뒤 반영 | review | obra/superpowers |
| [nextjs-bundle-optimizer](dev/performance/nextjs-bundle-optimizer/) | dev/performance | 측정→원인 분석→레시피 1개 적용 반복으로 Next.js 번들·빌드 시간 축소 | nextjs, bundle | pproenca/dot-skills |
| [performance-optimization](dev/performance/performance-optimization/) | dev/performance | 프론트·백엔드·쿼리 전반의 성능 문제를 측정 기반으로 최적화 | performance | addyosmani/agent-skills |
| [react-optimise](dev/performance/react-optimise/) | dev/performance | React Compiler·렌더링·번들·데이터 페칭 등 앱 단위 React 성능 최적화 | react, performance | pproenca/dot-skills |
| [accessibility](dev/web-quality/accessibility/) | dev/web-quality | WCAG 2.2 기준 웹 접근성 감사와 개선 | a11y, wcag | addyosmani/web-quality-skills |
| [best-practices](dev/web-quality/best-practices/) | dev/web-quality | 보안·호환성·코드 품질 관점의 최신 웹 개발 모범 사례 적용 | security, compatibility | addyosmani/web-quality-skills |
| [core-web-vitals](dev/web-quality/core-web-vitals/) | dev/web-quality | 필드·랩 데이터를 근거로 LCP·INP·CLS 개선 | cwv, lcp, inp, cls | addyosmani/web-quality-skills |
| [performance](dev/web-quality/performance/) | dev/web-quality | 로딩 속도·번들·리소스 최적화로 웹 성능 개선 | web-performance | addyosmani/web-quality-skills |
| [seo](dev/web-quality/seo/) | dev/web-quality | 메타 태그·구조화 데이터·사이트맵 등 검색 노출 최적화 | seo | addyosmani/web-quality-skills |
| [web-quality-audit](dev/web-quality/web-quality-audit/) | dev/web-quality | 성능·접근성·SEO·모범 사례를 근거 기반으로 종합 감사 | lighthouse, audit | addyosmani/web-quality-skills |
| [accessibility-compliance](dev/accessibility/accessibility-compliance/) | dev/accessibility | 모바일 접근성·포용적 디자인·보조기술 대응까지 포함한 WCAG 2.2 구현 | a11y, mobile | wshobson/agents |
| [accessibility-engineering](dev/accessibility/accessibility-engineering/) | dev/accessibility | 페이지·컴포넌트의 WCAG 2.2 AA 위반을 찾아 수정 | a11y, wcag | addyosmani/agent-skills |
| [improve-codebase-architecture](dev/architecture/improve-codebase-architecture/) | dev/architecture | 모듈을 깊게 만들 기회를 찾아 HTML 리포트로 제시하고 하나씩 검토 | architecture | mattpocock/skills |
| [setup-ts-deep-modules](dev/architecture/setup-ts-deep-modules/) | dev/architecture | dependency-cruiser로 TS 패키지를 deep module 구조로 강제 | typescript, dependency-cruiser | mattpocock/skills |
| [finishing-a-development-branch](dev/git-workflow/finishing-a-development-branch/) | dev/git-workflow | 구현 완료 후 머지/PR/정리 등 통합 방식 결정 | git, merge, pr | obra/superpowers |
| [using-git-worktrees](dev/git-workflow/using-git-worktrees/) | dev/git-workflow | 기능 작업을 격리된 git worktree에서 시작 | git, worktree | obra/superpowers |
| [diagram-design](non-dev/visualization/diagram-design/) | non-dev/visualization | 아키텍처·시퀀스·ER부터 차트·여정 지도까지 정돈된 다이어그램을 HTML/SVG/PNG로 생성 (Mermaid·draw.io 등 가져오기) | diagram, chart, svg | cathrynlavery/diagram-design |
| [diagnosing-superpowers](meta/diagnosing-superpowers/) | meta | superpowers 세션이 잘못 흘러간 원인을 사후 진단 | retrospective | obra/superpowers |
| [using-superpowers](meta/using-superpowers/) | meta | 대화 시작 시 skill을 찾아 먼저 호출하도록 하는 사용 규칙 | skill-usage | obra/superpowers |
| [writing-skills](meta/writing-skills/) | meta | 새 skill 작성·수정과 배포 전 동작 검증 | skill-authoring | obra/superpowers |
