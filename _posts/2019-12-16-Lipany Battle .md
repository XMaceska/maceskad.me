---
layout: post
title: "Abandoned village Musov"
image: /images/Musov_resized.jpg
SW: "3ds Max 2019, Lumion 9, Mudbox"
finished: 04.11.2019
lang: en
ref: musov

---


This is visualization of abandoned village Musov (Muschau). Village was flooded in year 1978 by water tank Nové Mlýny. Nowadays there is only small island with church left.

The surface of earth was obtained from vector-based model of contours Zabaged. Dimensions of building was measured from cadastral map and old photographs. Statues was moulded in Mudbox.
You can download whole modeling procedure text [here.](https://drive.google.com/file/d/12U5Q1p-7OHgOtkkkM6P-GssGBlXoA1Ia/view?usp=sharing) (czech language only)

It was my second paid job for National culture heritage (NAKI). 
Additional info about abandoned village is [here.](http://www.zaniklekrajiny.cz/atlas/modelova-uzemi/novomlynske-nadrze) (czech language only)
<br><br>
<h3> Interactive 3D model</h3>
<i>If 3D model is not loading, please turn off your Adblock.
<br>

You are able to jump in 3D model using green arrows. Fullscreen and VR mode is also supported (icons on right upper corner). In right-side panel you are able to find old cadastral map and place where this village was originally situtated.
<script async src="https://www.theasys.io/static/embed.js" data-theasys="vWEdS8mWRAgIomQAykG3TFmUqPPbpb" data-height="800"></script>
hosted with: Theasys.io
<br><br>
<h3> Renders </h3>
{% include image.html url="images/1M.jpg" caption="School" max_width="300px" align="center" %}
<br>
{% include image.html url="images/2M.jpg" caption="Ortstrasse" max_width="300px" align="center" %}
<br>
{% include image.html url="images/3M.jpg" caption="School and square" max_width="300px" align="center" %}
<br>
{% include image.html url="images/5M.jpg" caption="Church of saint Linhart" max_width="300px" align="center" %}
<br>
{% include image.html url="images/7M.jpg" caption="Townhall and statute of saint Jan Nepomucký" max_width="300px" align="center" %}
<br>
{% include image.html url="images/8M.jpg" caption="Church of saint Linhart" max_width="300px" align="center" %}
<br>
{% include image.html url="images/9M.jpg" caption="Church of saint Linhart, Orstrasse and statute of saint Jan Nepomucký" max_width="300px" align="center" %}
<br>
{% include image.html url="images/13M.jpg" caption="Square" max_width="300px" align="center" %}
<br>
{% include image.html url="images/15M.jpg" caption="Square from top" max_width="300px" align="center" %}
<br>
{% include image.html url="images/16M.jpg" caption="Village in rainy weather" max_width="300px" align="center" %}
<br>
{% include image.html url="images/17M.jpg" caption="Village in evening" max_width="300px" align="center" %}
<br>
{% include image.html url="images/21M.jpg" caption="Foggy weather" max_width="300px" align="center"  %}
<br>
{% include image.html url="images/12M.jpg" caption="School and rainy weather" max_width="300px" align="center" %}
<br>
{% include image.html url="images/23M.jpg" caption="Village in evening" max_width="300px" align="center" %}
<br>
{% include image.html url="images/25M.jpg" caption="Roof detail" max_width="300px" align="center" %}
<br>
{% include image.html url="images/4M.jpg" caption="Village from top" max_width="300px" align="center" %}
<br><br>
<h3> Compare 3D model with old photographs </h3>
When you left-click on image it will swap old photo with render
<p>
<img src="images/5M.jpg" alt="Square" id = "imgClickAndChange" />
<script>     
var images = ["images/5M.jpg", "images/5MO.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images[imgState];
});
</script> 
<p>
    <img alt="Townhall" src="images/6M.jpg"  id="imgClickAndChange2"   />
<script>     
var images2 = ["images/6M.jpg", "images/6MO.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange2");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images2[imgState];
});
</script> 
<p>
    <img alt="Square2" src="images/3M.jpg"  id="imgClickAndChange3"   />
<script>     
var images3 = ["images/3M.jpg", "images/3MO.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange3");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images3[imgState];
});
</script> 
<p>
    <img alt="Church" src="images/8M.jpg"  id="imgClickAndChange4"   />
<script>     
var images4 = ["images/8M.jpg", "images/8MO.JPG"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange4");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images4[imgState];
});
</script> 
<h3> Video </h3>
Fly-through village:
<br>
<iframe width="560" height="315" src="https://www.youtube.com/embed/NgXLj6BLhOU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>