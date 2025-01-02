---
layout: page
title: all posts
---

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small class="post-tags">
          {% for tag in post.tags %}
            <span class="tag">{{ tag }}</span>{% unless forloop.last %}, {% endunless %}
          {% endfor %}
        </small>
      </h3>
    </li>
  {% endfor %}
</ul> 