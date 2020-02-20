---
layout: page
title: Road cycling 
lang: cz
ref: road_cycling
permalink: /Road_cycling_cz/
---

Rád ovládám jakékoli rychlé kolo, které má berany. Jezdím už nějakou dobu a účastnil jsem se několika cyklokrosových, silničních i dráhových závodů. Kolo mi přijde fakt super a tak si díky tomuto nástroji dokáži vydělat občas i nějaký měšec plný peněz. Jezdím totiž jako messenger po Praze a práce to je, ale prací to nenazývám. Dojíždim na kole po Praze těměř vždy a všude. Občas nejenom po Praze, ale i po Čechách. 

Na Stravě mám vše:

<a style="display:inline-block;background-color:#FC4C02;color:#fff;padding:5px 10px 5px 30px;font-size:11px;font-family:Helvetica, Arial, sans-serif;white-space:nowrap;text-decoration:none;background-repeat:no-repeat;background-position:10px center;border-radius:3px;background-image:url('http://badges.strava.com/logo-strava-echelon.png')" href='http://strava.com/athletes/21086949' target="_clean">
  Follow me on <b>STRAVA</b>

<b>Heatmapa všech mých jízd se nachází [zde](https://maceskad.me/Road_cycling/heatmap)</b>



<h2>2019</h2>
Rok 2019 byl super, zbořil jsem minimálně dva rekordy. Najel jsem celkově 16 292 km za rok a taky jsem odjel z Prahy do Berlína za 19 a půl hodiny, čimž jsem si posunul svojí nejdelší jízdu za jediný den na hodnotu 417km.
<h3>Races</h3>
<ul class="listing">

{% for post in site.cycl_cz reversed %}
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

