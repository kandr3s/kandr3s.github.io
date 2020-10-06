---
layout: page
title: Recommended Films
permalink: films
---
 {% for film in site.data.films %}
<p>
{% if film.rating > "3.5" %}
<img class="log-icon" src="/images/cinema-fav.svg"><b>{{ film.name }} [{{ film.year }}]</b><br />{{ film.date }}{% endif %}
</p>
{% endfor %}