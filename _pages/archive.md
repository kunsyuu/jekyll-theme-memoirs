---
layout: page
title: Archive
permalink: /archive
comments: false
---

<div class="archive">

  {% comment %} 按年份分组并降序排列 {% endcomment %}
  {% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" | sort: 'name' | reverse %}
  
  {% for year in posts_by_year %}
    <div class="archive-year">
        <div class="year-header">
            <h2 id="{{ year.name }}">{{ year.name }}</h2>
            <span class="count">({{ year.items.size }})</span>
        </div>
      
      <ul class="archive-posts">
        {% comment %} 年度文章按日期降序排列 % for post in year.items reversed % {% endcomment %}
        {% for post in year.items %}
          <li>
            <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">
              {{ post.date | date: "%m-%d" }}
            </time>
            <a href="{{ post.url }}">{{ post.title }}</a>
          </li>
        {% endfor %}
      </ul>
    </div>
  {% endfor %}
</div>