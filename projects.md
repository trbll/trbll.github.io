---
layout: page
title: Projects
nav_order: 2
---

<ul class="post-list">
  {% for post in site.tags.project %}
    <li>
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul> 