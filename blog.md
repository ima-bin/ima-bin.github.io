---
layout: default
title: Blog
permalink: /blog/
---
<section class="section">
  <h1 class="h1">블로그 · Blog</h1>
  <p class="sub">디자인 인사이트, 실무 기록, 실험 노트를 정리합니다.</p>

  {% for post in site.posts %}
    <article class="card" style="margin-bottom:12px;">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p class="meta">{{ post.date | date: "%Y-%m-%d" }} · {{ post.lang_label }}</p>
      <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
    </article>
  {% endfor %}
</section>
