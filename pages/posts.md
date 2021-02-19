---
layout: page
title: Posts
permalink: /posts
---
Everything I say or share online.
<div class="legend">
<i class="far fa-comment-alt">Post</i>
<i class="far fa-newspaper">Tales</i>
<i class="far fa-images">Photos</i>
<i class="fab fa-spotify">Playlist</i><br />
<i class="fas fa-video">Video</i>
<i class="fas fa-record-vinyl">Tinta en las Cintas</i>
</div>
{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}{% if post.external_url %}<a class="post-title-link external" href="{{ post.external_url }}" target="_blank">{% else %}<a class="post-title-link" href="{{ post.url }}">{% endif %}{{ post.title }}</a><span class="post-date">{% include date.html %}</span>
    
</div>
{% endfor %}