---
layout: tintaenlascintas
title: "La vida es un mixtape"
description: "Tinta en las Cintas es el blog de música donde @kandr3s habla de los discos más influyentes en su vida."
permalink: /tintaenlascintas
---
<div class="grid-container">
  {% for post in site.posts %}
  {% if post.category == "Tinta en las Cintas" %}
  <article class="post-listing">
    <a class="post-title" href="{{ post.url }}">{{ post.title }}</a>
    <div class="album-art-container">
      <div class="album-art-frame">
        <img class="album-art" src="{% if post.feature %}{{ post.feature }}{% else %}{{ post.image }}{% endif %}" alt="{{ post.title }}">
      </div>
    </div>
  </article>
  {% endif %}
  {% endfor %}
</div>