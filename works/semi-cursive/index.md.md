---
title: 行楷作品 Semi-cursive Script
---
---
title: 行楷作品集 Semi-cursive Script
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="page-wrapper">

<h1>行楷作品集 Semi-cursive Script</h1>
<p class="section-note">
  行楷介于楷书与行书之间，是我创作与日常书写中使用最多的书体。
</p>

{% assign semi_images = site.static_files
  | where_exp: "file", "file.path contains '/works/semi-cursive/'" %}

<div class="gallery">
  {% for image in semi_images %}
    {% if image.extname == '.jpg' or image.extname == '.png' %}
    <figure class="gallery-item">
      <img src="{{ image.path | relative_url }}"
           alt="行楷作品 {{ forloop.index }}"
           loading="lazy">
      <figcaption class="gallery-item-caption">
        行楷作品 {{ forloop.index }}
      </figcaption>
    </figure>
    {% endif %}
  {% endfor %}
</div>

<p class="back-link">
  <a href="/index.html">← 返回首页</a>
</p>

</div>
