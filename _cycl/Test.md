---
layout: post
title: "Abandoned village Jablonec"
image: /images/jablonec_resized.jpg
categories: 3ds Max 2018, Lumion 8
finished: 11.9.2018
categories: cycl

---


This is visualization of abandoned village Jablonec (Ogfolderhaid)
Village was completely (even baroque church) destroyed in 1950s. there is millitary base at this moment. 

Earth surface was created from vector-based digital contour model Zabaged. Size of buildings was estimated from cadastral map and old photographies. 
Modelng procedure text is available [here.](https://drive.google.com/file/d/1w02unMZdq4FX71KxRKYxF9ETLqT3ZAy3/view?usp=sharing) (czech language only)

That was my first paid job for National Cultural heritage (NAKI)
Additional info about this village is [here.](http://www.zaniklekrajiny.cz/atlas/modelova-uzemi/boletice) (czech language only)

<h3> Renders </h3>
{% include image.html url="images/J1.jpg" caption="Parish church" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J2.jpg" caption="School" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J3.jpg" caption="Church from back" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J4.jpg" caption="Street and school" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J5.jpg" caption="Village-green" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J9.jpg" caption="Village-green from top" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J7.jpg" caption="Church from top" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J8.jpg" caption="Church from back" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J10.jpg" caption="Jablonec and Kmet hill" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J11.jpg" caption="Jablonec from north" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J12.jpg" caption="Church in evening" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J13.jpg" caption="Village-green in rainy weather" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J14.jpg" caption="Village-green from west" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J15.jpg" caption="Jablonec in winter" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J17.jpg" caption="Jablonec from top" max_width="300px" align="center" %}
<br><br>
<h3> Compare 3D model with old photographs </h3>
When you left-click on image it will swap old photo with render
<p>
    <img alt="Street"  src="images/J2.jpg" id = "imgClickAndChange" />
<script>     
var images = ["images/J2.jpg", "images/J2O.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images[imgState];
});
</script> 
<p>
    <img alt="Townhall" src="images/J9.jpg"  id="imgClickAndChange2"   />
<script>     
var images2 = ["images/J9.jpg", "images/J9O.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange2");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images2[imgState];
});
</script> 
<p>
    <img alt="Square2" src="images/J8.jpg"  id="imgClickAndChange3"   />
<script>     
var images3 = ["images/J8.jpg", "images/J8O.jpg"]

var imgState = 0;

var imgTag = document.getElementById("imgClickAndChange3");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images3[imgState];
});
</script> 

<h3> Video </h3>
Fly-through the village Jablonec
<iframe width="560" height="315" src="https://www.youtube.com/embed/yBfG8Soaxw4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>