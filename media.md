---
layout: page
title: media
---
Below is a sampling of the media that I've recently enjoyed or that has otherwise been important or influential to me. If it's on here, I'd likely recommend it.

### books
<div class="media-grid books">
{% for book in site.data.media.books %}
   <div class="media-item">
      <img src="{{ book.image }}" alt="{{ book.title }}">
      <p class="media-title">{{ book.title }}</p>
      <p class="media-attribution">{{ book.author }} ({{ book.year }})</p>
      <p class="media-notes">
         {{ book.status }}
         {% if book.links %}
         {% for link in book.links %}
         | <a href="{{ link.url }}" target="_blank">{{ link.text }}</a>
         {% endfor %}
         {% endif %}
      </p>
   </div>
{% endfor %}
</div>

### films
<div class="media-grid films">
{% for film in site.data.media.films %}
   <div class="media-item">
      <img src="{{ film.image }}" alt="{{ film.title }}">
      <p class="media-title">{{ film.title }}</p>
      <p class="media-attribution">({{ film.year }})</p>
      <p class="media-notes">{{ film.status }}{% if film.notes %}. {{ film.notes }}{% endif %}</p>
   </div>
{% endfor %}
</div>

### shows
<div class="media-grid tv">
{% for show in site.data.media.shows %}
   <div class="media-item">
      <img src="{{ show.image }}" alt="{{ show.title }} (Season {{ show.season }})">
      <p class="media-title">{{ show.title }}{% if show.season %} (Season {{ show.season }}){% endif %}</p>
      <p class="media-attribution">{{ show.network }} ({{ show.year }})</p>
      <p class="media-notes">{{ show.status }}</p>
   </div>
{% endfor %}
</div>

### albums
<div class="media-grid music">
{% for album in site.data.media.albums %}
   <div class="media-item">
      <img src="{{ album.image }}" alt="{{ album.title }} ({{ album.artist }})">
      <p class="media-title">{{ album.title }}</p>
      <p class="media-attribution">{{ album.artist }} ({{ album.year }})</p>
      <p class="media-notes">{{ album.notes }}</p>
   </div>
{% endfor %}
</div>