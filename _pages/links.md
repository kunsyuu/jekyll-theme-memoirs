---
layout: page
title: Links
permalink: /links
comments: true
image: "https://pic1.imgdb.cn/item/681f64bd58cb8da5c8eb7eeb.webp"
imageshadow: true
---

<div class="link-grid">
  {% for link in site.data.links %}
    <a href="{{ link.url }}" class="link-card" target="_blank">
      <div class="card-content">
        <h3>{{ link.name }}</h3>
        <p>{{ link.desc }}</p>
      </div>
    </a>
  {% endfor %}
</div>
