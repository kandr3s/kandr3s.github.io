---
layout: base
---
I'm @**kandr3s**...

* Programmer. Minimalist. Autodidact.
* Editor of [**Tinta en las Cintas**](https://tintaenlascintas.co/){:target="_blank"}.
* [Blogger](/posts) in 2021 🤓
* [FOSS](/tools) and privacy enthusiast. 
* Spacemen 3 [evangelist](https://tintaenlascintas.co/post/gospel){:target="_blank"}.

This website is a digital journal of all things like:
* [books](/books) read, 
* life-changing [albums](/music),
* loved [films](/films) and
* _everyday_ [tales](/tales).

#### My Links

{% for post in site.posts %}
<div class="post-info">{% include category-icons.html %}{% if post.external_url %}<a class="post-title-link external" href="{{ post.external_url }}" target="_blank">{% else %}<a class="post-title-link" href="{{ post.url }}">{% endif %}{{ post.title }}</a><span class="post-date">{% include date.html %}</span>
    
</div>
{% endfor %}

`Last updated February 12th 2021.`