# 3학년 기술 수업 사이트 모음 (수업 포털)

호원중학교 3학년 기술 · 2026학년도 2학기 수업에서 쓴 웹 사이트 10개를 수업 순서대로 한 쪽에 모은 정적 페이지.

- 포털 주소: https://ict-howon-portal.netlify.app
- 공개 저장소: https://github.com/techkwon/howon-class-portal
- 파일: `index.html` · `style.css` · `img/`(각 사이트 첫 화면, 800×500 webp)
- 빌드 없음 · 자바스크립트 없음 · 외부 글꼴 · 추적 도구 없음 · 다크 모드 지원

## 들어 있는 사이트

| 묶음 | 차시 | 사이트 | 주소 | 저장소 | 성취기준 |
|---|---|---|---|---|---|
| 수행평가 ① 포트폴리오 | 1 | 고장 난 카톡 사건 | https://ict-broken-katalk.netlify.app | `howon-broken-katalk` | [9기가04-15] |
| | 2 | 타임라인 대결 | https://ict-timeline-battle.netlify.app | `howon-timeline-battle` | [9기가04-16] |
| | 3 | 비행기 모드 실험 | https://ict-airplane-mode.netlify.app | `howon-airplane-mode` | [9기가04-16] |
| | 1~4 | 기술 탐사 수첩 도우미 | https://ict-notebook-guide.netlify.app | `howon-notebook-guide` | [9기가04-15] [9기가04-16] |
| 수행평가 ② 논술형 | 5 | 닿지 않은 집 | https://ict-unreached.netlify.app | `howon-unreached-house` | [9기가04-17] |
| | 6 | 같은 화면, 다른 조건 | https://ict-same-screen.netlify.app | `howon-same-screen` | [9기가04-17] |
| | 8 | 논술 쓰는 날 | https://ict-essay-check.netlify.app | `howon-essay-check` | [9기가04-17] |
| 교양 (성적 미반영) | 교양 8 | 호원버거 키오스크 챌린지 | https://ict-kiosk-challenge.netlify.app | `howon-burger-kiosk-challenge` | — |
| 수행평가 ③ 프로젝트 | 9~12 | 아이디어 공모전 | https://ict-idea-contest.netlify.app | `howon-idea-contest` | [9기가04-18] |
| 생명 기술 (평가 없음) | 13~16 | 생명 기술 대작전 | https://ict-bio-battle.netlify.app (진행판 `/host.html`) | `howon-bio-battle` | [9기가04-08] |

저장소는 모두 `https://github.com/techkwon/<저장소>` 이다. 채점 보고서(ict-jev-reliability)는 넣지 않는다.

## 고치는 법

- 카드 하나 = `index.html` 의 `<article class="card">` 하나. 복사해 제목 · 설명 · 주소만 바꾼다
- 혼자 있는 카드는 `card wide` 로 두면 큰 화면에서 가로로 넓게 보인다
- 단원 색은 `style.css` 맨 위 `--c1`~`--c5` (다크 모드 값은 그 아래 두 곳)

### 썸네일 다시 찍기

각 사이트 첫 화면을 1280×800 으로 찍어 800×500 webp 로 줄였다(Playwright + 설치된 Chrome, Pillow).
다시 찍으면 **학생 이름 · 학번 · 학생 글이 화면에 없는지 꼭 눈으로 확인**한다.

## 배포

```bash
netlify deploy --prod --no-build --dir . --site <site-id>
```

- Netlify 사이트 이름 `ict-howon-portal` · site id 는 아래 「배포 기록」
- 교사 PC 원본 폴더에는 git 이 없고, 이 저장소는 그 사본이다. 원본을 고치면 여기에 복사해 커밋 · 푸시한다

## 개인정보

포털에는 학생 이름 · 학번 · 학생 글 · 클래스룸 · 드라이브 · 패들렛 주소가 없다.
각 사이트의 개인정보 설명은 그 저장소 README 를 따른다.

## 배포 기록

- 2026-10-26 처음 만듦 · 배포
