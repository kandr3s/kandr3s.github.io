---
layout: page
title: Posts
permalink: /posts
---
Everything I say or share online.
<div class="legend">
<i class="far fa-comment-alt"></i><span>Posts</span>
<i class="far fa-newspaper"></i><span>Tales</span>
<i class="far fa-images"></i><span>Photos</span>
<i class="fab fa-spotify"></i><span>Playlist</span><br />
<i class="fas fa-video"></i><span>Video</span>
<i class="fas fa-record-vinyl"></i><span>On Music</span>
</div>
{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}{% if post.external_url %}<a class="post-title-link external" href="{{ post.external_url }}" target="_blank">{% else %}<a class="post-title-link" href="{{ post.url }}">{% endif %}{{ post.title }}</a><span class="post-date">{% include date.html %}</span>
    
</div>
{% endfor %}