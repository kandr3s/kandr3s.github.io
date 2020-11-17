---
layout: page
title: Books I Read
permalink: /books
---
Most books I've read over the past few years. Favorite ones hightlighted.
{% for book in site.data.books %}
{% if book.rating > "4" %}
<span><i class="fas fa-bookmark fa-2x"></i></span><b>{{ book.name }}</b><br />
{{ book.author }}{% else %}
<span><i class="far fa-bookmark fa-2x"></i></span>{{ book.name }}<br />
{{ book.author }}
{% endif %} 
{% endfor %}