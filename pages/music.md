---
layout: page
title: Music I ❤
permalink: /music
---
This is the music that's shaped my life, albums I consider treasures.

I try to expand on the importance of Rock albums at [**Tinta en las Cintas**](https://tintaenlascintas.co){: class="external" target="_blank"}, a blog in Spanish about music we're passionated about.

Here's a chronological list of my most important records.  

<code>
Last Updated {% last_modified_at %}
</code>

#### Personal Treasures
{% for album in site.data.records %}
<p class="log-list">
    {% if album.rating == "10" or album.rating =="9" %}
    <i class="category-icon fas fa-record-vinyl"></i><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}

#### Amazing Albums
{% for album in site.data.records %}
 <p class="log-list">
    {% if album.rating == "8" %}
    <i class="category-icon fas fa-compact-disc"></i><b>{{ album.title }}</b> [{{ album.year }}]<br />
    {{ album.artist }}
    {% endif %}
</p>
{% endfor %}