---
layout: page
title: Road cycling
permalink: /Road_cycling/
---
I am riding all kinds of fast bikes with handlebars. I have already competed several cyclo-cross, road, and track races. I am also bike messenger and I am commuting on bike anywhere in town and mostly if its possible anywhere in Czechia. 
Feel free to follow me on Strava:

<a style="display:inline-block;background-color:#FC4C02;color:#fff;padding:5px 10px 5px 30px;font-size:11px;font-family:Helvetica, Arial, sans-serif;white-space:nowrap;text-decoration:none;background-repeat:no-repeat;background-position:10px center;border-radius:3px;background-image:url('http://badges.strava.com/logo-strava-echelon.png')" href='http://strava.com/athletes/21086949' target="_clean">
  Follow me on
  <img src='http://badges.strava.com/logo-strava.png' alt='Strava' style='margin-left:2px;vertical-align:text-bottom' height=13 width=51 />
</a>

<h2>2019</h2>
That was great year in cycling, I did 16 292 km, which is my personal record. Also did my longest trip in one sigle ride - 417 km.
<h3>Races</h3>
<ul class="listing">
{% for post in site.cycl %}
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

