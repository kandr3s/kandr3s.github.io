---
layout: playlist
title: "Sintiembres"
date: "2020-11-03"
permalink: /playlist/sintiembres
category: "Playlist"
image: /images/playlist-sintiembres.jpg
spotify: https://open.spotify.com/playlist/0bLFWaincDOz1HSzneQXPT
---
### Tracklist
{% for track in site.data.playlists.sintiembres %}
<div class="tracklist">
    <img style="float: left; width: 68px; margin-right: 10px" class="track-image" src="{{ track.image }}" />
    <p class="track-title">{{ track.title }}</p>
    <p class="track-artist">{{ track.artist }}</p>
    <p class="page-link track-preview"><a href="{{ track.preview }}" target="_blank">Preview</a></p>
</div>
{% endfor %}



