---
layout: page
title: Road cycling 
lang: cz
ref: road_cycling
permalink: /Road_cycling_cz/
---

Rád ovládám jakékoli rychlé kolo, které má berany. Jezdím už nějakou dobu a účastnil jsem se několika cyklokrosvých, silnicních i dráhových závodů. KOlo mi přijde fakt super a tak si díky tomuto nástroji dokáži vydělat občas i inějaký měšec plný peněz. Jezdím totiž jako messenger po Praze a práce to je, ale prací to nenazývám. Dojíždim na kole po Praze těmř vždy a všude a občas, pokud je to alespoň trochu možné, dojíždím i kamkoliv po Čechách na kole. 

Na Stravě mám vše:

<a style="display:inline-block;background-color:#FC4C02;color:#fff;padding:5px 10px 5px 30px;font-size:11px;font-family:Helvetica, Arial, sans-serif;white-space:nowrap;text-decoration:none;background-repeat:no-repeat;background-position:10px center;border-radius:3px;background-image:url('http://badges.strava.com/logo-strava-echelon.png')" href='http://strava.com/athletes/21086949' target="_clean">
  Follow me on <b>STRAVA</b>


<h3> Heatmapa mých jízd </h3>

<meta name="viewport" content="width=device-width,initial-scale=1">
<script src='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.js'></script>
<link href='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.css' rel='stylesheet' />

    
<style>
    #map {
   	width: 1200px;
  	 height: 600px; }
</style>



<!--// map --> 
<script src='https://api.mapbox.com/mapbox.js/plugins/leaflet-omnivore/v0.2.0/leaflet-omnivore.min.js'></script>
<div id='map'></div>

<script>
L.mapbox.accessToken = 'pk.eyJ1IjoibWFjZXNrYSIsImEiOiJjazVhMDFmbGgxMmxnM21wZ3BvNjJhdXMzIn0.OC2jBDlbR4AE1rhBzI__cQ';
var map = L.mapbox.map('map',"mapbox.dark")

var rideStyle = {
    "color": "#ff6600",
    "weight": 2,
    "opacity": .2,
}
customLayerRide = L.geoJson(null, {
    style: rideStyle
}).addTo(map);
    
    

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_4.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_5.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_6.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_7.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_8.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_9.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_10.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_11.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_12.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
    
    
//<!--// data GPX -->   
//    for (var i = 1; i < 4; i++){
//            var runLayer = omnivore.gpx('GPX/' + i.toString() + ".gpx", null, customLayerRide)
//                .on('ready', function() {
//                    map.fitBounds(runLayer.getBounds());
//            })
//            .addTo(map);    
//        }
//var runLayer = omnivore.gpx("2.gpx",null,customLayerRide)
//    .addTo(map);
//var runLayer = omnivore.gpx("3.gpx",null,customLayerRide)
//    .addTo(map);
        
</script>




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

