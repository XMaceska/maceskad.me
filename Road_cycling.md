---
layout: page
title: Road cycling
permalink: /Road_cycling/
---

<html>
<head> 
    <meta charset="UTF-8">
    <title>Leaflet gpx plugin basic</title>
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.3.4/dist/leaflet.css"
   integrity="sha512-puBpdR0798OZvTTbP4A8Ix/l+A4dHDD0DGqYW6RQ+9jxkRFclaxxQb/SJAWZfWAkuyeQUytO7+7N4QKrDh+drA=="
   crossorigin=""/>
   <style> 
  	#map {
   	width: 700px;
  	 height: 600px; }
	</style> 
  </head>
  <body>
    
    <script src="https://unpkg.com/leaflet@1.3.4/dist/leaflet.js"
   integrity="sha512-nMMmRyTVoLYqjP9hrbed9S+FzjZHW5gY1TWCHA5ckwXZBadntCNs8kEqAWdrb9O7rxbCaA4lKTIWjDXZxflOcA=="
   crossorigin=""></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet-gpx/1.4.0/gpx.min.js"></script>
    <div id ="map"> </div> 
    <script>
    var map = L.map('map', 	{center: [42.4624, -6.2073],zoom: 11});

	L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png').addTo(map);

  var url = 'demo.gpx'; // URL al archivo GPX 
  new L.GPX(url, {async: true}).on('loaded', function(e) {
    map.fitBounds(e.target.getBounds());
  }).addTo(map);
	</script>
  </body>
</html>

I am riding all kinds of fast bikes with handlebars. I have already competed several cyclo-cross, road, and track races. I am also bike messenger and I am commuting on bike anywhere in town and mostly if its possible anywhere in Czechia. 
Feel free to follow me on Strava:

<a style="display:inline-block;background-color:#FC4C02;color:#fff;padding:5px 10px 5px 30px;font-size:11px;font-family:Helvetica, Arial, sans-serif;white-space:nowrap;text-decoration:none;background-repeat:no-repeat;background-position:10px center;border-radius:3px;background-image:url('http://badges.strava.com/logo-strava-echelon.png')" href='http://strava.com/athletes/21086949' target="_clean">
  Follow me on <b>STRAVA</b>


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

