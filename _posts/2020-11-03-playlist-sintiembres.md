---
layout: post
title: "Sintiembres"
date: "2020-11-03"
permalink: /playlist/sintiembres
category: "Playlists"
---
<img src="/images/playlist-sintiembres.jpg" />

<span class="page-link"><a class="external" href="https://open.spotify.com/playlist/0bLFWaincDOz1HSzneQXPT" target="_blank">Spotify</a></span>

### Tracklist
{% for track in site.data.playlists.sitiembres %}
<div class="tracklist">
    <img class="track-image" src="{{ track.image }}" />
    <p class="track-title">{{ track.title }}</p>
    <p class="track-artist">{{ track.artist }}</p>
</div>
{% endfor %}



