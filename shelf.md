---
layout: page
title: shelf
---
<nav class="shelf-nav">
  <a href="#books">books</a> •
  <a href="#films">films</a> •
  <a href="#shows">shows</a> •
  <a href="#albums">albums</a> •
  <a href="#games">games</a>
</nav>

Below is a sampling of the media that I've recently enjoyed or that has otherwise been important or influential to me. If it's on here, I'd likely recommend it. Will hopefully keep this up to date.

### <span id="books">books</span> <a href="#" class="back-to-top">↑</a>
<div class="media-grid books">
{% for item in site.data.media.books %}
   <div class="media-item">
      <img src="{{ item.image }}" alt="{{ item.title }}">
      <p class="media-title">{{ item.title }}</p>
      <p class="media-attribution">{{ item.attribution }}</p>
      <p class="media-notes">
         {{ item.note }}
         {% if item.links %}
         {% for link in item.links %}
         | <a href="{{ link.url }}" target="_blank">{{ link.text }}</a>
         {% endfor %}
         {% endif %}
      </p>
   </div>
{% endfor %}
</div>

### <span id="films">films</span> <a href="#" class="back-to-top">↑</a>
<div class="media-grid films">
{% for item in site.data.media.films %}
   <div class="media-item">
      <img src="{{ item.image }}" alt="{{ item.title }}">
      <p class="media-title">{{ item.title }}</p>
      <p class="media-attribution">{{ item.attribution }}</p>
      <p class="media-notes">{{ item.note }}</p>
   </div>
{% endfor %}
</div>

### <span id="shows">shows</span> <a href="#" class="back-to-top">↑</a>
<div class="media-grid tv">
{% for item in site.data.media.shows %}
   <div class="media-item">
      <img src="{{ item.image }}" alt="{{ item.title }}">
      <p class="media-title">{{ item.title }}</p>
      <p class="media-attribution">{{ item.attribution }}</p>
      <p class="media-notes">{{ item.note }}</p>
   </div>
{% endfor %}
</div>

### <span id="albums">albums</span> <a href="#" class="back-to-top">↑</a>
<div class="media-grid music">
{% for item in site.data.media.albums %}
   <div class="media-item">
      <img src="{{ item.image }}" alt="{{ item.title }}">
      <p class="media-title">{{ item.title }}</p>
      <p class="media-attribution">{{ item.attribution }}</p>
      <p class="media-notes">{{ item.note }}</p>
   </div>
{% endfor %}
</div>

### <span id="games">games</span> <a href="#" class="back-to-top">↑</a>
<div class="media-grid games">
{% for item in site.data.media.games %}
   <div class="media-item">
      <img src="{{ item.image }}" alt="{{ item.title }}">
      <p class="media-title">{{ item.title }}</p>
      <p class="media-attribution">{{ item.attribution }}</p>
      <p class="media-notes">{{ item.note }}</p>
   </div>
{% endfor %}
</div>