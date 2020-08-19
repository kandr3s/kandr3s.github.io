---
layout: page
title: Books
permalink: /books
---
{% for book in site.data.books %}
<p>
{% if book.rating > "4" %}
<span><i class="fas fa-bookmark"></i></span><b>{{ book.name }}</b><br />
{{ book.author }}{% else %}
<span><i class="far fa-bookmark"></i></span>{{ book.name }}<br />
{{ book.author }}
{% endif %} 
</p>
{% endfor %}