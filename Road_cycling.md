---
layout: page
title: Road cycling
permalink: /Road_cycling/
---

<html>
<head>
<meta charset=utf-8 />
<title>GPX trackpoints and waypoints</title>
<meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
<script src='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.js'></script>
<link href='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.css' rel='stylesheet' />
    
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/noUiSlider/8.5.1/nouislider.min.css" /> <!--// slider -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/noUiSlider/8.5.1/nouislider.min.js"></script> <!--// slider -->
    
<style>
  body { margin:0; padding:0; }
  #map { position:absolute; top:0; bottom:0; width:100%; }
</style>
</head>
<body>
<!--// slider -->
<div id="slider" style="top: 0px; right: 1px; margin: 10px 25px;"></div>
<div style="margin-right: auto; margin-left: auto; width: 90%; margin-bottom: 10px; text-align: center;">
<input type="number" min='1' max='3' id="input-number-min">
<input type="number" min='2' max='3' id="input-number-max">
</div>
    
<!--// map --> 
<script src='https://api.mapbox.com/mapbox.js/plugins/leaflet-omnivore/v0.2.0/leaflet-omnivore.min.js'></script>
<div id='map'></div>

<script>
L.mapbox.accessToken = 'pk.eyJ1IjoibWFjZXNrYSIsImEiOiJjazVhMDFmbGgxMmxnM21wZ3BvNjJhdXMzIn0.OC2jBDlbR4AE1rhBzI__cQ';
var map = L.mapbox.map('map',"mapbox.dark")

var rideStyle = {
    "color": "#ff6600",
    "weight": 3,
    "opacity": .1,
}
customLayerRide = L.geoJson(null, {
    style: rideStyle
}).addTo(map);
    
    
var runLayer = omnivore.gpx('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/1.gpx',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.gpx('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/2.gpx',null, customLayerRide)
    .on('ready', function() {
        map.fitBounds(runLayer.getBounds());
    })
    .addTo(map);
var runLayer = omnivore.gpx('https://raw.githubusercontent.com/XMaceska/maceskad.me/master/GPX/3.gpx',null, customLayerRide)
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
    
    
    
<!--// slider -->
var slidervar = document.getElementById('slider');
noUiSlider.create(slidervar, {
    connect: true,
    start: [ 1, 3 ],
    range: {
        min: 1,
        max: 3
    }
});
    
document.getElementById('input-number-min').setAttribute("value", 1);
document.getElementById('input-number-max').setAttribute("value", 3);

var inputNumberMin = document.getElementById('input-number-min');
var inputNumberMax = document.getElementById('input-number-max');
inputNumberMin.addEventListener('change', function(){
    slidervar.noUiSlider.set([this.value, null]);
});
inputNumberMax.addEventListener('change', function(){
    slidervar.noUiSlider.set([null, this.value]);
});

slidervar.noUiSlider.on('update', function( values, handle ) {
    //handle = 0 if min-slider is moved and handle = 1 if max slider is moved
    if (handle==0){
        document.getElementById('input-number-min').value = values[0];
    } else {
        document.getElementById('input-number-max').value =  values[1];
    }
//we will definitely do more here...wait
})
rangeMin = document.getElementById('input-number-min').value;
rangeMax = document.getElementById('input-number-max').value;

cluster_popplaces.clearLayers();
//and repopulate it
popplaces = new L.geoJson(exp_popplaces,{
    onEachFeature: pop_popplaces,
        filter:
            function(feature, layer) {
                 return (feature.properties.pop_max <= rangeMax) && (feature.properties.pop_max >= rangeMin);
            },
    pointToLayer: popplaces_marker
})
//and back again into the cluster group
cluster_popplaces.addLayer(popplaces);
        
</script>
</body>
</html>

TED I am riding all kinds of fast bikes with handlebars. I have already competed several cyclo-cross, road, and track races. I am also bike messenger and I am commuting on bike anywhere in town and mostly if its possible anywhere in Czechia. 
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

