---
layout: page
title: Heatmap
lang: en
ref: heatmap
permalink: /Road_cycling/heatmap
---


<meta name="viewport" content="initial-scale=1,maximum-scale=1,user-scalable=no">
<script src='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.js'></script>
<link href='https://api.mapbox.com/mapbox.js/v3.2.1/mapbox.css' rel='stylesheet' />

<style>
    body { margin: 100; padding: 100; }
    #map { position: absolute; top: 0; bottom: 0; height: 80%; width: 70%; }
</style>




<!--// map --> 
<script src='https://api.mapbox.com/mapbox.js/plugins/leaflet-omnivore/v0.2.0/leaflet-omnivore.min.js'></script>
<script src='https://api.mapbox.com/mapbox.js/plugins/leaflet-fullscreen/v1.0.1/Leaflet.fullscreen.min.js'></script>
<link href='https://api.mapbox.com/mapbox.js/plugins/leaflet-fullscreen/v1.0.1/leaflet.fullscreen.css' rel='stylesheet' />

<div id='map'></div>

<script>
L.mapbox.accessToken = 'pk.eyJ1IjoibWFjZXNrYSIsImEiOiJja2d1ejZ3NWsweWMzMnZtajhubXRsMGN5In0.rkCvV1tI5xFxTqGuGNh3eQ';
var map = L.mapbox.map('map',"mapbox.dark")
L.control.fullscreen().addTo(map);



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

