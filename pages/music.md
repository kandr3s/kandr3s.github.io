---
layout: page
title: Music Pages
permalink: /music
---
{% for album in site.data.albums %}
 <p class="log-list">
            {% if album.rating > "7" %}
            <img class="log-icon" src="/images/vinyl-fav.svg"><b>{{ album.title }} [{{ album.year }}]</b><br />
            {{ album.artist }}{% else %}
            <img class="log-icon" src="/images/vinyl.svg">{{ album.title }} [{{ album.year }}]<br />
            {{ album.artist }}
            {% endif %}
</p>
{% endfor %}