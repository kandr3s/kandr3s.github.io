---
layout: page
title: Posts
permalink: /posts
---
<div class="legend">
    <i class="fab fa-microblog"></i><span class="legend-text">Blog</span>
    <i class="far fa-images"></i><span class="legend-text">Photos</span>
    <i class="fab fa-spotify"></i><span class="legend-text">Playlists</span>
    <i class="fas fa-video"></i><span class="legend-text">Video</span><br />
    <img style="width: 18px; height: 18px; padding: 0; margin: 0;" src="images/typewriter.svg"><span class="legend-text">Tales</span>
    <img style="width: 18px; height: 18px; padding: 0; margin: 0;" src="images/tintaenlascintas.svg"><span class="legend-text">Tinta en las Cintas</span>
</div>
{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}{% if post.external_url %}<a class="post-title-link external" href="{{ post.external_url }}" target="_blank">{% else %}<a class="post-title-link" href="{{ post.url }}">{% endif %}{{ post.title }}</a><span class="post-date">{% include date.html %}</span>
    
</div>
{% endfor %}