---
layout: page
title: Posts
permalink: /posts
---
This I've said or shared online.

<div class="legend">
    <i class="fab fa-microblog"></i><span class="legend-text">Post</span>
    <i class="fab fa-spotify"></i><span class="legend-text">Playlist</span>
    <i class="fas fa-video"></i><span class="legend-text">Video</span>
    <img style="width: 18px; height: 18px; padding: 0; margin: 0;" src="images/typewriter.svg"><span class="legend-text">Tales</span>
    <img style="width: 18px; height: 18px; padding: 0; margin: 0;" src="images/tintaenlascintas.svg"><span class="legend-text">On Music</span>
</div>
{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}<a class="post-title-link {% if post.category == 'Tinta en las Cintas' %}external{% endif %}" href="{{ post.url }}">{{ post.title }}</a><span class="post-date">{{ post.category }} - {% include date.html %}</span>
</div>
{% endfor %}