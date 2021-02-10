---
layout: page
title: Records I ❤
permalink: /music
---
The music that shaped my life, real treasures I consider worth your time.

In Chronological order.
`Updated Feb 10th 2020`

#### Treasures
{% for album in site.data.records %}
<p class="log-list">
    {% if album.rating == "10" or album.rating =="9" %}
    <img class="log-icon" src="/images/vinyl-fav.svg"><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}

#### Recommended
{% for album in site.data.records %}
 <p class="log-list">
    {% if album.rating == "8" %}
    <img class="log-icon" src="/images/vinyl.svg"><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}