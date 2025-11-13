---
title: 小楷作品 Xiaokai
---
---
title: 小楷作品集 Xiaokai
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="page-wrapper">

<h1>小楷作品集 Xiaokai</h1>
<p class="section-note">
  小楷更像一场缓慢的冥想，需要耐心与时间，是我最喜欢的修心式书写。
</p>

{% assign xiaokai_images = site.static_files
  | where_exp: "file", "file.path contains '/works/xiaokai/'" %}

<div class="gallery">
  {% for image in xiaokai_images %}
    {% if image.extname == '.jpg' or image.extname == '.png' %}
    <figure class="gallery-item">
      <img src="{{ image.path | relative_url }}"
           alt="小楷作品 {{ forloop.index }}"
           loading="lazy">
      <figcaption class="gallery-item-caption">
        小楷作品 {{ forloop.index }}
      </figcaption>
    </figure>
    {% endif %}
  {% endfor %}
</div>

<p class="back-link">
  <a href="/index.html">← 返回首页</a>
</p>

</div>
