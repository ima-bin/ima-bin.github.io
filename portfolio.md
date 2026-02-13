---
layout: default
title: Portfolio
permalink: /portfolio/
---
<section class="section">
  <h1 class="h1">포트폴리오 · Portfolio</h1>
  <p class="sub">문제 정의 → 가설 설정 → 디자인 실행 → 결과 검증의 흐름으로 정리했습니다.</p>

  <div class="grid">
    {% assign projects = site.projects | sort: 'order' %}
    {% for p in projects %}
      <a class="card" href="{{ p.url | relative_url }}">
        <span class="thumb-wrap">
          {% if p.thumbnail %}
            <img src="{{ p.thumbnail | relative_url }}" alt="{{ p.title }} thumbnail" style="width:100%;height:170px;object-fit:cover;display:block;" />
          {% else %}
            <span class="thumb">Project Preview</span>
          {% endif %}
        </span>
        <h3>{{ p.title }}</h3>
        <p class="meta">{{ p.period }} · {{ p.role }}</p>
        <p>{{ p.summary }}</p>
      </a>
    {% endfor %}
  </div>
</section>
