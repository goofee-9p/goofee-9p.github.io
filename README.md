# goofee-9p — Letters

> ## ✋ 먼저 읽어주세요 — Read me first
>
> **이 저장소에 글을 쓰거나(레터·작업 추가) 디자인·스타일을 바꾸기 전에, 반드시
> [`DESIGN.md`](DESIGN.md)를 먼저 읽어 주세요.** 색·타이포·간격·컴포넌트 등 모든 시각
> 결정의 단일 기준(source of truth)입니다. `style.css`는 그 토큰을 그대로 구현할 뿐이므로,
> 무언가를 바꾸려면 **DESIGN.md에서 먼저 정하고** `style.css`의 `:root`에 반영하세요.
>
> - 📄 **[DESIGN.md](DESIGN.md)** — 이 사이트의 디자인 토큰 + 근거 (꼭 먼저 볼 것)
> - 📚 **[docs/design-md-spec.md](docs/design-md-spec.md)** — DESIGN.md 포맷을 읽고 쓰는 법
>   (Google Labs 원본 스펙). 다른 프로젝트에 이 방식을 쓸 때도 여기서 꺼내 쓰면 됩니다.
> - 🤖 AI 에이전트(Claude Code 등)는 [`CLAUDE.md`](CLAUDE.md)에 같은 지침이 있습니다.

개인 레터이자 포트폴리오 공간. GitHub Pages로 배포되는 정적 사이트입니다.
오래 남는 생각을 편지(Letter)처럼 적어 모으고, 선별한 작업(Work)을 함께 둡니다.

## 디자인

디자인 시스템은 [`DESIGN.md`](DESIGN.md)에 정의되어 있습니다 (Google Labs의
DESIGN.md 포맷). 한 줄 요약: **에디토리얼 레터** — 세리프 타이포, 넉넉한 여백,
헤어라인, 따뜻한 모노크롬 + 절제된 테라코타 액센트. 색·타이포·간격 토큰은 모두
`DESIGN.md`의 YAML front matter가 기준이며, `style.css`가 이를 CSS 변수로 구현합니다.

## 구조

```
index.html              홈 (최신 레터 중심)
style.css               전체 스타일 (디자인 토큰 → CSS 변수)
DESIGN.md               디자인 시스템 원본(source of truth)
pages/
  letters.html          레터 아카이브
  work.html             포트폴리오 (항목은 placeholder — 실제 내용으로 교체)
  about.html            소개
  questions.html        답을 비워 둔 질문들
  contact.html          연락처
posts/
  ax-dashboard-to-operating-system.html   Letter 003
  closed-loop-ai-native.html              Letter 002
  prompt-agent-thinking.html              Letter 001
```

## 콘텐츠 추가

- **새 레터:** `posts/`에 글 HTML을 추가하고, `pages/letters.html`과 (최신 글이면)
  `index.html`의 목록에 한 줄 추가합니다. 글 번호는 `Letter 00N` 형식.
- **작업:** `pages/work.html`의 `.work-item` 블록을 복제해 채웁니다 (파일 상단 주석 참고).
- **디자인 변경:** 색/타이포/간격은 `DESIGN.md`에서 정한 뒤 `style.css`의 `:root`
  변수에 반영합니다.

## 배포

GitHub 저장소 `Settings > Pages`에서 `Deploy from a branch` → `main` 브랜치 `/root`.
사용자 페이지 저장소이므로 도메인은 `goofee-9p.github.io` 입니다.
