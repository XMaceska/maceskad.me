---
layout: page
title: 3D modeling
ref: 3D_modeling
lang: cz
permalink: /3D_modelace/
---



Tvořím 3D vizualizaci reálných i nereálných objektů. of real or unreal objects. On that page you can find all my projects I did or I am working on.


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

