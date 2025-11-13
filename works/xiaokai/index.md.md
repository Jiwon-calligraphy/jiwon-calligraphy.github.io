---
title: 小楷作品 Xiaokai
---

<link rel="stylesheet" href="/assets/style.css">

# 小楷作品集 Xiaokai

小楷需要耐心与时间，是我最喜欢的“静心书写”。

---

## 精选作品 Selected Works

<div class="gallery">
{% assign xiaokai_images = site.static_files
  | where_exp: "file", "file.path contains '/works/xiaokai/'"
%}

{% for image in xiaokai_images %}
  {% if image.extname == '.jpg' or image.extname == '.png' or image.extname == '.jpeg' %}
  <figure class="work-card">
    <img src="{{ image.path | relative_url }}" alt="小楷作品">
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
