---
layout: page
title: Books I Read
permalink: /books
---
Most books I've read in recent years. Favorites are highlighted.

`Updated March 31st 2021`
{% for book in site.data.books %}
{% if book.rating > '4' %}<i class="category-icon fas fa-bookmark"></i>{% else %}
<i class="category-icon far fa-bookmark"></i>{% endif %}<b>{{ book.name }}</b><br />
{{ book.author }}

{% endfor %}