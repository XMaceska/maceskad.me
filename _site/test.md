<!DOCTYPE html>
<html>

<head>
    <meta charset='utf-8' />
    <title>Display a map</title>
    <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
    <!-- Mapbox -->
    <script src='https://api.tiles.mapbox.com/mapbox-gl-js/v0.50.0/mapbox-gl.js'></script>
    <link href='https://api.tiles.mapbox.com/mapbox-gl-js/v0.50.0/mapbox-gl.css' rel='stylesheet' />

    <!-- Slider -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/noUiSlider/11.1.0/nouislider.min.css" />
    <script src='https://cdnjs.cloudflare.com/ajax/libs/noUiSlider/11.1.0/nouislider.min.js'></script>

    <!-- Moment.js -->
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.22.1/moment.min.js"></script>
    <style>
    body {
        margin: 0;
        padding: 0;
    }

    #map {
        position: absolute;
        top: 0;
        bottom: 0;
        width: 100%;
    }

    .slider-control-container {
        padding: 5px;
    }

    .slider-control-range-display {
        font-size: 18px;
        padding-top: 5px;
        padding-bottom: 5px;
        font-weight: 700;
    }

    /*
    class to change color
    .noUi-connect {
        background: #2980b9;
    }
    */
    </style>
</head>

<body>
    <div id='map'></div>
    <script src="rangeSlider.js"></script>
    <script>
    mapboxgl.accessToken = 'pk.eyJ1IjoibWFjZXNrYSIsImEiOiJjazVhMDFmbGgxMmxnM21wZ3BvNjJhdXMzIn0.OC2jBDlbR4AE1rhBzI__cQ';
    var map = new mapboxgl.Map({
        container: 'map', // container id
        style: 'mapbox://styles/mapbox/streets-v9', // stylesheet location
        center: [-121.5, 44.0], // starting position [lng, lat]
        zoom: 6 // starting zoom
    });

    var sliderOptions = {
        elm: 'slider-control',
        layer: 'demo',
        source: 'demo',
        input: true,
        controlWidth: '400px',
        minProperty: 'Start',
        maxProperty: 'End',
        sliderMin: '1965-01-01T08:00:00.000Z',
        sliderMax: '2025-12-31T08:00:00.000Z',
        filterMin: '1985-11-28T08:00:00.000Z',
        filterMax: '2005-01-01T08:00:00.000Z',
        propertyType: 'iso8601',
        rangeDescriptionFormat: 'shortDate',
        descriptionPrefix: 'Date:'
    }

    map.addControl(new RangeSlider(sliderOptions, 'top-right'));

    map.on('load', function() {
        map.addSource('demo', { type: 'geojson', data: 'https://devdata.ntendril.com/6493abf0497911e8b1091ff5c85a4d37.json' })
        map.addLayer({
            'id': 'demo',
            'source': 'demo',
            'type': 'fill',
            'paint': {
                'fill-color': '#C676C6',
                'fill-outline-color': '#000',
                'fill-opacity': 0.7
            }
        });
    })

    </script>
</body>

</html>