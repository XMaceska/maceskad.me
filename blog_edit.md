---
layout: page
title: Blog
lang: cz
ref: blog
permalink: /blog/
---
Na tomto místě se nachází měsíčník obsahující souhrn určitých informací a situací, které se odehrály v konkrétním měsíci.
Blog je psán spíše odlehčeným stylem, než neodlehčeným. 
<ul class="listing">
{% for post in site.blo reversed %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
    <a href="{{ post.url | prepend: site.baseurl }}">
    <img src="{{ post.image | prepend: site.baseurl }}" alt="{{ post.title }}" title="{{ post.title }}"> <a href="{{ post.url | prepend: site.baseurl }}">
  <li class="listing-item">
    <time datetime="{{ "post.date" | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url | prepend: site.baseurl }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
