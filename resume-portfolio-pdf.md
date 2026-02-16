---
layout: default
title: Resume PDF
permalink: /resume/portfolio-pdf/
page_count: 52
---

<section class="section">
  <h1 class="h1">포트폴리오</h1>

  <div style="display:grid; gap:18px; max-width:980px; margin:16px auto 0;">
    {% for i in (1..page.page_count) %}
      {% assign num = i | prepend: '00' | slice: -2, 2 %}
      <figure class="card" style="margin:0; padding:10px;">
        <img src="{{ '/assets/images/resume-pdf-260214/page-' | append: num | append: '.jpg' | relative_url }}"
             alt="포트폴리오 페이지 {{ i }}"
             style="width:100%; height:auto; display:block; border-radius:10px;"
             loading="{% if i == 1 %}eager{% else %}lazy{% endif %}" />
        <figcaption class="meta" style="margin-top:8px;">Page {{ i }}</figcaption>
      </figure>
    {% endfor %}
  </div>
</section>
