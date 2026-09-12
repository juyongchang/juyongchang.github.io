# AGENTS.md

이 저장소는 Kwangwoon University Computer Vision Lab의 GitHub Pages 홈페이지이다.

사이트 주소:

`https://juyongchang.github.io`

현재 목표는 기존 Google Sites 홈페이지

`https://sites.google.com/site/juyongchang/`

를 Jekyll 기반 GitHub Pages로 이전하고 유지보수하는 것이다.

## 기본 원칙

- 현재 단계에서는 **migration을 우선하고 redesign은 최소화한다.**
- 기존 홈페이지의 구조, 내용, 메뉴 순서, 표현을 최대한 유지한다.
- 확인되지 않은 정보는 임의로 추가하거나 추측하지 않는다.
- 기존 문구를 특별한 이유 없이 rewrite하거나 요약하지 않는다.
- 단순하고 읽기 쉬운 academic homepage 스타일을 유지한다.
- 유지보수하기 쉬운 구조를 우선한다.
- 불필요한 기능과 dependency를 추가하지 않는다.

## 사이트 구조

기본 top-level 메뉴는 다음 순서를 유지한다.

1. Home
2. Research
3. Students
4. Publications

현재 단계에서는 새로운 top-level 메뉴를 임의로 추가하지 않는다.

## 기술 스택

- GitHub Pages
- Jekyll
- Markdown
- HTML
- CSS

가능하면 GitHub Pages가 기본 지원하는 Jekyll 기능만 사용한다.

다음은 특별한 이유가 없는 한 사용하지 않는다.

- React
- Vue
- Astro
- Bootstrap
- Tailwind CSS
- 복잡한 JavaScript
- 외부 Jekyll plugin
- 별도의 GitHub Actions 배포 workflow

JavaScript 사용은 가능한 한 최소화한다.

## 디자인 원칙

기존 Google Sites와 유사한 단순한 연구실 홈페이지 스타일을 유지한다.

- 흰색 배경
- 텍스트 중심
- 단순한 navigation
- 적절한 여백
- 읽기 쉬운 typography
- desktop/mobile responsive
- 최대 콘텐츠 폭 약 900~1000px

다음과 같은 요소는 가급적 사용하지 않는다.

- 과도한 animation
- gradient
- 큰 hero banner
- 과도한 shadow
- 불필요한 card UI
- 일반 기업용 landing page 같은 디자인

기존 사이트보다 약간 깔끔하게 다듬는 것은 가능하지만 전체적인 성격을 바꾸지 않는다.

## 기존 콘텐츠 이전

기존 홈페이지의 실제 내용을 기준으로 작업한다.

- 텍스트를 가능한 한 그대로 유지한다.
- 사람 이름, 논문 제목, 연도, 이메일, 프로젝트 기간 등을 정확히 확인한다.
- 논문과 프로젝트 정보를 임의로 수정하지 않는다.
- 기존 링크가 있으면 가능한 한 유지한다.
- 기존 이미지는 가능한 경우 `assets/images/`에 저장하여 사용한다.
- 이미지를 확보할 수 없으면 임의의 placeholder 이미지를 만들지 않는다.
- 확인되지 않는 내용은 TODO로 남긴다.

## Publications

논문 목록은 단순성과 유지보수성을 우선한다.

현재 규모에서 Markdown으로 충분하면 별도의 복잡한 데이터베이스 구조를 만들지 않는다.

검색, 필터링, JavaScript 기반 publication UI 등은 명시적인 요청이 없는 한 추가하지 않는다.

## Students

`Students` 메뉴 이름을 유지한다.

현재 학생과 졸업생의 정보를 기존 홈페이지 기준으로 유지한다.

학생 이름, 과정, 이메일, 졸업 연도, 현재 소속 등을 임의로 변경하거나 추가하지 않는다.

## 코드 수정 원칙

- 기존 구조를 먼저 이해한 후 수정한다.
- 가능한 한 작은 범위로 수정한다.
- 단순한 문제를 해결하기 위해 전체 구조를 크게 변경하지 않는다.
- 같은 코드나 스타일을 불필요하게 중복하지 않는다.
- 새로운 파일이나 dependency를 추가할 때는 실제 필요성이 있는지 먼저 판단한다.
- 기존 동작을 깨지 않도록 한다.

## 검증

변경 후 가능하면 다음을 확인한다.

- Jekyll build 오류 여부
- 내부 링크
- 외부 링크
- 이미지 경로
- navigation
- desktop/mobile layout
- 한글 Unicode 깨짐 여부

가능하면 다음 명령으로 build를 확인한다.

```bash
bundle exec jekyll build
```

## 작업 완료 시

작업 후 다음 내용을 간략하게 보고한다.

- 수정한 파일
- 주요 변경 사항
- build 결과
- 확인하지 못한 사항
- TODO

## 핵심 원칙

**Keep it simple.**

**Migration first, redesign later.**

**기존 홈페이지의 정보를 임의로 바꾸지 않는다.**
