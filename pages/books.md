---
layout: page
title: Books I Read
permalink: /books
---
Most books I've read in recent years. Favorites are highlighted.

<code>
Last Updated {% last_modified_at %}
</code>

{% for book in site.data.books %}
{% if book.rating > '3.5' %}<i class="category-icon fas fa-bookmark"></i>{% else %}
<i class="category-icon far fa-bookmark"></i>{% endif %}<b>{{ book.name }}</b><br />
{{ book.author }}

{% endfor %}