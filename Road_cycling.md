---
layout: page
title: Road cycling
lang: en
ref: road_cycling
permalink: /Road_cycling/
---

I am riding all kinds of fast bikes with handlebars. I have already competed several cyclo-cross, road, and track races. I am also bike messenger and I am commuting on bike anywhere in town and mostly if its possible anywhere in Czechia. 
Feel free to follow me on Strava:

<a style="display:inline-block;background-color:#FC4C02;color:#fff;padding:5px 10px 5px 30px;font-size:11px;font-family:Helvetica, Arial, sans-serif;white-space:nowrap;text-decoration:none;background-repeat:no-repeat;background-position:10px center;border-radius:3px;background-image:url('http://badges.strava.com/logo-strava-echelon.png')" href='http://strava.com/athletes/21086949' target="_clean">
  Follow me on <b>STRAVA</b>


<h3> Heatmap of my rides </h3>

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
    
    

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_4_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_5_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_6_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_7_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_8_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_9_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_10_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_11_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2017_12_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_1_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_2_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_3_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_4_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_5_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_6_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_7_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_8_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_9_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_10_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_11_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2018_12_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
  
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_1_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_2_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_3_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_4_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_5_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_6_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_7_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_8_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_9_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_10_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
    
var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_11_resized.json',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);

var runLayer = omnivore.geojson('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2019_12_resized.json',null, customLayerRide)
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
That was great year in cycling, I did 16 292 km, which is my personal record. Also did my longest trip in one sigle ride - 417 km.
<h3>Races</h3>
<ul class="listing">

{% for post in site.cycl reversed %}
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

