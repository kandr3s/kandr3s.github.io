---
layout: base
---
I'm <span class="highlight">@<b>`kandr3s`</b></span> <span class="page-link">Colombian / Minimalist / Autodidact</span>

This is my personal space on the Internet. Here I share everything I post on the Internet.

<div class="legend">
    <i class="fab fa-microblog"></i><span class="legend-text">Post</span>
    <i class="fab fa-spotify"></i><span class="legend-text">Playlist</span>
    <i class="fas fa-video"></i><span class="legend-text">Video</span>
    <i class="far fa-file-alt"></i><span class="legend-text">Tales</span><br />
    <img style="width: 18px; height: 18px; padding: 0; margin: 0;" src="images/tintaenlascintas.svg"><span class="legend-text"><a href="/tintaenlascintas">Tinta en las Cintas</a></span>
</div>
{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}<a class="post-title-link {% if post.redirect_to %}external{% endif %}" href="{{ post.url }}">{{ post.title }}</a><span class="post-date">{{ post.category }} - {% include date.html %}</span>
</div>
{% endfor %}
