# 블로그를 가장 쉽게 쓰는 방법 (GitHub Pages)

이 사이트는 Jekyll 기반이라, **`_posts`에 Markdown 파일 1개 추가**하면 글이 올라갑니다.

## 1) 새 글 만들기

파일명 규칙:

`YYYY-MM-DD-slug.md`

예시:

`2026-02-16-my-first-post.md`

## 2) 맨 위에 메타 정보(front matter) 붙이기

```md
---
title: "글 제목"
date: 2026-02-16 11:00:00 +0900
lang_label: "KO"
---
```

## 3) 본문 작성

Markdown으로 작성하면 됩니다.

```md
짧은 소개 문장

## 소제목

- 포인트 A
- 포인트 B
```

## 4) 배포

GitHub에 커밋/푸시하면 자동 배포됩니다.

```bash
git add _posts/2026-02-16-my-first-post.md
git commit -m "Add blog post: my first post"
git push
```

## 빠른 시작

`_posts/_template.md`를 복사해서 파일명만 날짜 규칙에 맞춰 바꿔 쓰세요.
