---
layout: page
title: Films I ❤
permalink: films
---
These are the movies I've watched over the years that I consider worth your time.

{% for film in site.data.films %}
<p>
{% if film.rating > "4" %}
<img class="log-icon" src="/images/cinema-fav.svg"><b>{{ film.name }} [{{ film.year }}]</b><br />dir. {{ film.director }}{% endif %}
</p>
{% endfor %}