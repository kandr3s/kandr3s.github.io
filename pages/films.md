---
layout: page
title: Films I ❤
permalink: films
---
These are the movies I've watched over the years that I consider worth your time.
You can also check my [Letterboxd](https://letterboxd.com/kandr3s){: .external target="_blank"} profile for more films I've enjoyed.

<code>
Last Updated {% last_modified_at %}
</code>

{% for film in site.data.films %}
<p>
{% if film.rating >= "4" %}
<i class="category-icon fas fa-film"></i><b>{{ film.name }} [{{ film.year }}]</b><br />dir. {{ film.director }}{% endif %}
</p>
{% endfor %}