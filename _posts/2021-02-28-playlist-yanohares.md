---
layout: post
title: "Yanoharés"
date: "2021-02-28"
permalink: /playlist/yanohares
category: "Playlists"
playlist: "yanohares"
---

<img src="/images/playlist-yanohares.jpg" />

<span class="page-link"><a class="external" href="https://open.spotify.com/playlist/5TgmyeJaqoclHSSp72Z69P" target="_blank">Spotify</a></span>

The turn of the year, the "magical change" we all expect. 
2020 is gone and all the things I was to do remain to do.
Familiar sounds for days that pile on top of each other.  
"I won't do anymore."

### Tracklist
{% for track in site.data.playlists.yanohares %}
<div class="tracklist">
    <img class="track-image" src="{{ track.image }}" />
    <p class="track-title">{{ track.title }}</p>
    <p class="track-artist">{{ track.artist }}</p>
</div>
{% endfor %}



