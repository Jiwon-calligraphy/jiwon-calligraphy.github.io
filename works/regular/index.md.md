---
title: 楷书作品 Regular Script
---
---
title: 楷书作品集 Regular Script
---

<link rel="stylesheet" href="/assets/css/style.css">

<div class="page-wrapper">

<h1>楷书作品集 Regular Script</h1>
<p class="section-note">
  安静、克制、有分寸感的楷书，是我书写训练的基本功。
</p>

{% assign regular_images = site.static_files
  | where_exp: "file", "file.path contains '/works/regular/'" %}

<div class="gallery">
  {% for image in regular_images %}
    {% if image.extname == '.jpg' or image.extname == '.png' %}
    <figure class="gallery-item">
      <img src="{{ image.path | relative_url }}"
           alt="楷书作品 {{ forloop.index }}"
           loading="lazy">
      <figcaption class="gallery-item-caption">
        楷书作品 {{ forloop.index }}
      </figcaption>
    </figure>
    {% endif %}
  {% endfor %}
</div>

<p class="back-link">
  <a href="/index.html">← 返回首页</a>
</p>

</div>
