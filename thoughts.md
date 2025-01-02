---
layout: page
title: thoughts
---

<ul class="post-list">
  {% for post in site.tags.thought %}
    <li>
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul> 