---
title: 楷书作品 Regular Script
---
---
title: 楷书作品 Regular Script
---

<link rel="stylesheet" href="/assets/style.css">

# 楷书作品集 Regular Script

楷书是我长期练习的基本书体，结构端正，笔画清晰，是学习书法的根基。

---

## 精选作品 Selected Works

<div class="gallery">
{% assign regular_images = site.static_files
  | where_exp: "file", "file.path contains '/works/regular/'" %}
{% for image in regular_images %}
  {% assign ext = image.extname | downcase %}
  {% if ext == '.jpg' or ext == '.jpeg' or ext == '.png' %}
  <figure class="work-card">
    <img src="{{ image.path | relative_url }}" alt="楷书作品 {{ forloop.index }}">
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
