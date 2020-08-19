---
layout: page
title: Films
permalink: films
---
 {% for film in site.data.films limit:25 %}
<p>
{% if film.tv == "1" %}<img class="log-icon" src="/images/tv.svg">{% elsif film.rating > "3.5" %}
<img class="log-icon" src="/images/cinema-fav.svg"><b>{{ film.name }} [{{ film.year }}]</b>{% else %}<img class="log-icon" src="/images/cinema.svg">{{ film.name }} [{{ film.year }}]{% endif %}<br />
{{ film.date }}</p>
{% endfor %}