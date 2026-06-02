# goofee-9p.github.io — 작업 지침 (read this first)

개인 **레터 + 포트폴리오** 정적 사이트. GitHub Pages (`main` 브랜치 = 배포).

## ✋ 무엇이든 만들기 전에: DESIGN.md를 먼저 읽으세요

이 저장소에서 **콘텐츠를 추가하거나(레터·작업) 디자인/스타일을 바꾸기 전에, 반드시
[`DESIGN.md`](DESIGN.md)를 읽고 그 토큰을 기준으로** 작업하세요. 이건 선택이 아니라 전제입니다.

- **`DESIGN.md` = 디자인 시스템의 단일 기준(source of truth).** YAML front-matter 토큰
  (`colors` / `typography` / `spacing` / `rounded` / `components`)은 **정답값**이고,
  아래 마크다운 프로즈는 **근거와 적용 지침**입니다. (Google Labs의 DESIGN.md 포맷)
- **`style.css`는 그 토큰을 `:root` CSS 변수로 구현할 뿐입니다.** 무언가를 바꾸려면
  **DESIGN.md를 먼저 고치고**, 그 변경을 `style.css`의 `:root`에 반영하세요. 둘을 어긋나게
  두지 마세요.
- DESIGN.md **포맷 자체**(읽고 쓰는 법)가 궁금하면 [`docs/design-md-spec.md`](docs/design-md-spec.md).

## 톤 유지 (요약 — 자세한 건 DESIGN.md)

- 에디토리얼 **레터** 무드: 세리프(Newsreader + Noto Serif KR), 라벨만 Inter 대문자, 넉넉한 여백, 헤어라인.
- **따뜻한 모노크롬 + 절제된 테라코타 액센트 `#B5512E`** 하나만. 액센트는 아주 소량(레터 번호·링크·짧은 룰)만. **2차 색·그림자 금지.**
- 한글 본문은 세리프로. 한 화면에 액센트는 몇 군데를 넘기지 않기.

## 콘텐츠/구조

- 추가 방법(새 레터, Work 항목)은 [`README.md`](README.md) 참고.
- 레터(=에세이) 본문 글은 **함부로 고치지 말고 보존**하세요. 레이아웃/구조만 디자인 규칙에 맞춥니다.
- `pages/work.html`의 작업 항목은 아직 **placeholder** — 실제 내용으로 채울 곳.

## 배포

`main`에 푸시하면 GitHub Pages가 자동 빌드합니다. 사용자 페이지라 도메인은
`goofee-9p.github.io`. 빌드 스텝/번들러 없음 — 순수 HTML/CSS.
