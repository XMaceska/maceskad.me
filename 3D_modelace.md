---
layout: page
title: 3D modelace
ref: 3D_modeling
lang: cz
permalink: /3D_modelace/
---



Zabývám se tvorbou 3D modelů, ať už reálných ale i ne objektů. Tady na tomhle místě se nachází mé portfolio s projekty, které jsem tvořil sám a nebo v týmu. Seřazeno podle data dokončení.


<ul class="listing">
{% for post in site.posts_cz reversed %}
  {% capture y %}{{post.date | date:"%Y" }}{% endcapture %}
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

