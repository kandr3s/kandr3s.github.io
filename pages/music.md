---
layout: page
title: Records I ❤
permalink: /music
---
The music that shaped my life, real treasures I consider worth your time.

In chronological order.
`Updated Feb 10th 2020`

#### Treasures
{% for album in site.data.records %}
<p class="log-list">
    {% if album.rating == "10" or album.rating =="9" %}
    <i class="category-icon fas fa-record-vinyl"></i><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}

#### Recommended
{% for album in site.data.records %}
 <p class="log-list">
    {% if album.rating == "8" %}
    <i class="category-icon fas fa-compact-disc"></i><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}