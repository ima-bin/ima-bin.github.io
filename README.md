# 임아빈 포트폴리오/블로그 (GitHub Pages + Jekyll)

취업용 디자이너 포트폴리오를 위한 최소 구조 템플릿입니다.

## 사이트 컨셉
- **목표**: 디자이너 취업용 포트폴리오
- **톤**: 미니멀 (블랙 중심)
- **구성**: 블로그 + 포트폴리오 분리
- **언어**: 한국어 / 영어

## 메뉴 구조
- Home (`/`)
- Portfolio (`/portfolio/`)
- Blog (`/blog/`)
- About (`/about/`)
- Resume (`/resume/`)
- Contact (`/contact/`)

## 포함된 더미 콘텐츠
- About 한/영 소개 문구
- 프로젝트 3개 더미
- 경력/활동/수상/자격증 더미
- 블로그 글 KO/EN 샘플

## 본인 정보로 교체할 파일
1. `index.md` - 메인 카피
2. `_projects/*.md` - 프로젝트 상세
3. `about.md` - 소개
4. `resume.md` - 경력/수상/자격증
5. `_posts/*.md` - 블로그 글
6. `assets/images/` - 프로필/썸네일 이미지

## 프로젝트 설명 문구 템플릿 (복붙용)

### KO
- **프로젝트명**:
- **한 줄 요약**: 무엇을 왜 개선했는지
- **기간/역할**:
- **문제 정의**: 어떤 사용자 문제/비즈니스 문제였는지
- **가설**: 어떤 변화가 어떤 지표를 올릴 것이라 봤는지
- **디자인 접근**: 리서치/와이어/비주얼/프로토타이핑
- **성과**: 수치 중심(전환율, 이탈률, CTR, CPA 등)
- **배운 점**: 다음 프로젝트에 어떻게 반영했는지

### EN
- **Project**:
- **Summary**:
- **Period / Role**:
- **Problem**:
- **Hypothesis**:
- **Design Approach**:
- **Outcome (Metrics)**:
- **Learnings**:

## 로컬 실행
```bash
bundle exec jekyll serve
```

## GitHub Pages 배포
1. 저장소 이름을 `ima-bin.github.io`로 생성
2. 이 폴더 내용 업로드
3. GitHub 저장소 Settings → Pages에서 Branch `main` / root 선택
4. 배포 완료 후 `https://ima-bin.github.io` 접속

## 다음 추천 작업
- 프로필 사진 업로드 후 홈/어바웃에 반영
- 프로젝트 썸네일 제작 후 카드에 적용
- 각 프로젝트에 문제/과정/결과(숫자) 강화
