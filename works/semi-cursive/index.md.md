---
title: 行楷作品 Semi-cursive
---

<link rel="stylesheet" href="/assets/style.css">

# 行楷作品集 Semi-cursive

行楷介于楷书与行书之间，是我日常书写中最常用的书体。

---

## 精选作品 Selected Works

<div class="gallery">
{% assign semi_images = site.static_files
  | where_exp: "file", "file.path contains '/works/semi-cursive/'"
%}

{% for image in semi_images %}
  {% if image.extname == '.jpg' or image.extname == '.png' or image.extname == '.jpeg' %}
  <figure class="work-card">
    <img src="{{ image.path | relative_url }}" alt="行楷作品">
    <figcaption class="work-caption">
      行楷习作 · {{ forloop.index }}
    </figcaption>
  </figure>
  {% endif %}
{% endfor %}
</div>

<div class="back-home">
  <a href="/index.html">← 返回首页</a>
</div>
