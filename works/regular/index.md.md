---
title: 楷书作品 Regular Script
---

<link rel="stylesheet" href="/assets/style.css">

# 楷书作品集 Regular Script

安静、克制、有留白感的楷书，是我书写训练的基本功。

---

## 精选作品 Selected Works

<div class="gallery">
{% assign regular_images = site.static_files
  | where_exp: "file", "file.path contains '/works/regular/'"
%}

{% for image in regular_images %}
  {% if image.extname == '.jpg' or image.extname == '.png' or image.extname == '.jpeg' %}
  <figure class="work-card">
    <img src="{{ image.path | relative_url }}" alt="楷书作品">
    <figcaption class="work-caption">
      楷书习作 · {{ forloop.index }}
    </figcaption>
  </figure>
  {% endif %}
{% endfor %}
</div>

<div class="back-home">
  <a href="/index.html">← 返回首页</a>
</div>
