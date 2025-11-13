---
title: 小楷作品 Xiaokai
---
---
title: 小楷作品 Xiaokai
---

<link rel="stylesheet" href="/assets/style.css">

# 小楷作品集 Xiaokai

小楷精致细腻、字形紧凑，是我风格中偏文雅的一支。多用于诗文誊写与题字创作。

---

## 精选作品 Selected Works

<div class="gallery">
{% assign xiaokai_images = site.static_files
  | where_exp: "file", "file.path contains '/works/xiaokai/'" %}
{% for image in xiaokai_images %}
  {% assign ext = image.extname | downcase %}
  {% if ext == '.jpg' or ext == '.jpeg' or ext == '.png' %}
  <figure class="work-card">
    <img src="{{ image.path | relative_url }}" alt="小楷作品 {{ forloop.index }}">
    <figcaption class="work-caption">
      小楷习作 · {{ forloop.index }}
    </figcaption>
  </figure>
  {% endif %}
{% endfor %}
</div>

<div class="back-home">
  <a href="/index.html">← 返回首页</a>
</div>
