---
layout: page
title: media
---
Below is a sampling of the media that I've recently enjoyed or that has otherwise been important or influential to me. If it's on here, I'd likely recommend it.

### books
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

### films
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

### shows
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

### albums
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