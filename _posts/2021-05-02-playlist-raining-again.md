---
layout: playlist
title: "Raining Again"
date: "2021-05-02"
permalink: /playlist/raining-again
category: "Playlist"
image: /images/playlist-raining-again.jpg
spotify: https://open.spotify.com/playlist/6VDpLDUOmzAPi47m4IECIU
---
Rains all over Medellín again.  
The country is in chaos.  
Here's nothing but guitar sounds.

### Tracklist
{% for track in site.data.playlists.raining-again %}
<div class="track-info">
    <img style="float: left; width: 68px; margin-right: 10px" class="track-image" src="{{ track.image }}" />
    <p class="track-title">{{ track.title }}</p>
    <p class="track-artist">{{ track.artist }}</p>
    <p class="page-link track-preview"><a href="{{ track.preview }}" target="_blank">Preview</a></p>
</div>
{% endfor %}

Art: iidamiidam