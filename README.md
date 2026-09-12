# CVLAB @ KWU

Kwangwoon University Computer Vision Lab 홈페이지입니다. GitHub Pages와 Jekyll로 구성되어 있으며, 기존 Google Sites 홈페이지의 내용을 이전해 관리합니다.

## 파일 구성

- `index.md`: Home
- `research.md`: Research 및 프로젝트
- `students.md`: 재학생과 졸업생
- `publications.md`: 논문 및 특허
- `_layouts/default.html`, `_includes/header.html`: 공통 레이아웃과 내비게이션
- `assets/css/style.css`: 공통 스타일
- `assets/images/`: 홈페이지 이미지

## 로컬 실행

Ruby와 Bundler가 설치된 환경에서 다음 명령을 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://localhost:4000`을 엽니다. 각 페이지의 내용은 해당 Markdown 파일에서 수정하고, 이미지는 `assets/images/`에 추가합니다.
