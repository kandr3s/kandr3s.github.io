---
layout: base
---
I'm <span class="highlight">@`kandr3s`</span>, a Colombian programmer that lives a minimalist life, owning only essential stuff and using open source [tools](/tools). 

I studied journalism and computer science but haven't received a college degree. I've worked in gold mines, retail, warehouses, call centers, online publications and writing code. I consider myself an autodidact as I've become this person thanks to curiosity, love for learning and being fortunate enough to have grown up with a screen connected to the Internet.

<img class="portrait" src="images/me.jpg" alt="kandr3s profile picture" />

I'm not an active social media user so this website aims to be my <a href="/feed.xml" alt="kandr3s RSS Feed" title="kandr3s RSS Feed"><span class="highlight">main channel</span></a> for [**communicating**](/now){: title="/Now Page"} with the world online. This is my personal space on the Web, the place for me to share [**thoughts**](#posts) and ideas, [**books**](/books) read, loved [**films**](/films) and life-changing [**music**](/music).

Write to me at <a href="mailto:hello@kandr3s.co"><span class="highlight">`hello`@`kandr3s.co`</span></a> or follow me elsewhere on:

<ul class="menu">
    <li class="page-link"><a href="/spotify">Spotify</a></li>
    <li class="page-link"><a href="/letterboxd">Letterboxd</a></li>
    <li class="page-link"><a href="/rym">RateYourMusic</a></li>
    <!--li class="page-link"><a href="/mixcloud">Mixcloud</a></li-->
</ul>

<h2 id="posts" class="content-title">Posts</h2>

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
