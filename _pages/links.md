---
layout: page
title: 友情链接
permalink: /links
comments: true
;image: "https://pic1.imgdb.cn/item/681f64bd58cb8da5c8eb7eeb.webp"
imageshadow: true
---
<div class="link-grid">
  {% for link in site.data.links %}
    <a href="{{ link.url }}" 
       class="link-card" 
       style="--bg-img: url('{{ link.img }}')" 
       target="_blank"
       rel="noopener noreferrer">
      <div class="card-content">
        <h3>{{ link.name }}</h3>
        <p>{{ link.desc }}</p>
      </div>
    </a>
  {% endfor %}
</div>

如果你愿意的话，欢迎留下信息添加友情链接。你的网站有持续更新内容就行。

```yaml
- name: Sail's Blog
  url: https://warn.im/
  desc: 一个社恐的博客
  img: https://img.loliapi.cn/i/pp/img122.webp
  ```
