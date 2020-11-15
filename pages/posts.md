---
layout: page
title: Posts
permalink: /posts
---

{% for post in site.posts %}
{% if post.external_url == null %}
<div class="posts">
<a href="{{ post.url }}">
   <h2>{{ post.title }}</h2>
    {% include date.html %}
    {% if post.description %}
    <p class="post-description">{{ post.description }}</p>
    {% endif %}
</a>
</div>
{% endif %}
{% endfor %}
