---
layout: page
title: Road cycling
permalink: /Road_cycling/
---
I am riding all kinds of fast bikes with handlebars. I have already competed several cyclo-cross, road, and track races. I am also bike messenger and I am commuting on bike anywhere in town and mostly if its possible anywhere in Czechia. 
<h3>2019</h3>
I did two road races.
 - firstly it was UAC Prague-Doksy, which is quite short race (73km) from Prague to town Doksy. I have already did is year ago and this year I really looked forward for this event. 

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture cycl %}{{ category | first }}{% endcapture %}
    <div id="#{{ cycl | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
Feel free to follow me on Strava:
<style>
  .strava-badge- { display: inline-block; height: 48px; }
  .strava-badge- img { visibility: hidden; height: 48px; }
  .strava-badge-:hover { background-position: 0 -63px; }
  .strava-badge-follow { height: 48px; width: 48px; background: url(//badges.strava.com/echelon-sprite-48.png) no-repeat 0 0; }
</style>
<a href="http://strava.com/athletes/21086949" class="strava-badge- strava-badge-follow" target="_blank"><img src="//badges.strava.com/echelon-sprite-48.png" alt="Strava" /></a>