---
layout: default
title: Archive
---
<h1 class="page-title">~/archive</h1>

<div class="archive-list">
  {% for post in site.posts %}
  <div class="archive-item">
    <span class="archive-date">{{ post.date | date: "%Y-%m-%d" }}</span>
    <span class="archive-arrow">→</span>
    <a href="{{ post.url | relative_url }}" class="archive-link">{{ post.title }}</a>
  </div>
  {% endfor %}
</div>
