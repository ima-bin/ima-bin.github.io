---
layout: default
title: Portfolio
permalink: /portfolio/
---
<section class="section">
  <h1 class="h1">포트폴리오 · Portfolio</h1>
  <p class="sub">프로젝트 썸네일은 추후 교체 예정입니다.</p>

  <div class="grid">
    {% assign projects = site.projects | sort: 'order' %}
    {% for p in projects %}
      <a class="card" href="{{ p.url | relative_url }}">
        {% if p.thumbnail %}
          <img class="thumb" src="{{ p.thumbnail | relative_url }}" alt="{{ p.title }} thumbnail" style="object-fit:cover;width:100%;height:180px;" />
        {% else %}
          <div class="thumb">Thumbnail Placeholder</div>
        {% endif %}
        <h3>{{ p.title }}</h3>
        <p class="meta">{{ p.period }} · {{ p.role }}</p>
        <p>{{ p.summary }}</p>
      </a>
    {% endfor %}
  </div>
</section>
