---
layout: playlist
title: "Yanoharés"
date: "2021-02-28"
permalink: /playlist/yanohares
category: "Playlist"
image: /images/playlist-yanohares.jpg
spotify: https://open.spotify.com/playlist/5TgmyeJaqoclHSSp72Z69P
---
The turn of the year, the "magical change" we all expect. 
2020 is gone and all the things I was to do remain to do.
Familiar sounds for days that pile on top of each other.  
"I won't do anymore."

### Tracklist
{% for track in site.data.playlists.yanohares %}
<div class="track-info">
    <img style="float: left; width: 68px; margin-right: 10px" class="track-image" src="{{ track.image }}" />
    <p class="track-title">{{ track.title }}</p>
    <p class="track-artist">{{ track.artist }}</p>
    <p class="page-link track-preview"><a href="{{ track.preview }}" target="_blank">Preview</a></p>
</div>
{% endfor %}
