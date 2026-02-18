---
layout: default
title: Blog
permalink: /blog/
---
<section class="section blog-page">
  <h1 class="h1">블로그 · Blog</h1>
  <p class="sub">디자인 인사이트, 실무 기록, 실험 노트를 정리합니다.</p>

  <div class="blog-hero card">
    <p class="blog-hero-kicker">Latest notes</p>
    <p class="blog-hero-text">
      문제를 정의하고, 실험하고, 검증한 과정을 기록합니다.
      읽고 바로 실무에 적용할 수 있는 형태로 정리하는 것을 목표로 합니다.
    </p>
  </div>

  <div class="blog-list">
    {% for post in site.posts %}
      <article class="card blog-card">
        <a class="blog-link" href="{{ post.url | relative_url }}">
          <div class="blog-main">
            <div class="blog-copy">
              <h3>{{ post.title }}</h3>
              <p class="meta">{{ post.date | date: "%Y-%m-%d" }}{% if post.lang_label %} · {{ post.lang_label }}{% endif %}</p>
              <p class="blog-excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>
              <span class="blog-read">Read article →</span>
            </div>
            {% if post.og_image %}
              <div class="blog-thumb-wrap">
                <img class="blog-thumb no-zoom" src="{{ post.og_image | relative_url }}" alt="{{ post.title }} 썸네일" loading="lazy">
              </div>
            {% endif %}
          </div>
        </a>
      </article>
    {% endfor %}
  </div>
</section>
