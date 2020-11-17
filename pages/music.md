---
layout: page
title: Records I ❤
permalink: /music
---
The music that shaped my life, real treasures I consider worth your time.

{% for album in site.data.albums %}
 <p class="log-list">
            {% if album.rating > "7" %}
            <img class="log-icon" src="/images/vinyl-fav.svg"><b>{{ album.title }}</b> [{{ album.year }}]<br />
            {{ album.artist }}
            {% endif %}
</p>
{% endfor %}