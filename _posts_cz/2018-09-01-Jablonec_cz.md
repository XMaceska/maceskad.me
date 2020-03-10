---
layout: post_cz
title: "Zaniklá obec Jablonec"
image: /images/jablonec_resized.jpg
SW: 3ds Max 2018, Lumion 8
finished: 11.9.2018
lang: cz
ref: jablonec

---


Jedná se o vizualizaci zaniklé obce Jablonec (Ogfolderhaid). Vesnice, včetně barokního kostela byla zničena v letech okolo roku 1950. Nyní se na tomto místě nachází vojenská základna s tankovou střílnou. 

Povrch země modelu byl vytvořen z digitálního vektorového modelu vrstevnic Zabaged. Velikost budov byla odhadnuta z dobových fotografií a změřena ze starých katastrálních map. Celý proces modelace je dostupný [zde.](https://drive.google.com/file/d/1w02unMZdq4FX71KxRKYxF9ETLqT3ZAy3/view?usp=sharing)

V tomto případě se jednalo o mojí první placenou zakázku pro katedru aplikované geografie, spolupracující s ministerstvem kultury. Projekt vznikl jako program na podporu aplikovaného výzkumu a vývoje národní a kulturní identity (NAKI). Více informací o obci lze najít [zde.](http://www.zaniklekrajiny.cz/atlas/modelova-uzemi/boletice)

<h3> Rendery </h3>
{% include image.html url="images/J1.jpg" caption="Farní kostel" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J2.jpg" caption="Škola" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J3.jpg" caption="Kostel zezadu" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J4.jpg" caption="Ulice a škola" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J5.jpg" caption="Náves" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J9.jpg" caption="Náves seshora" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J7.jpg" caption="Kostel shora" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J8.jpg" caption="Kostel zezadu" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J10.jpg" caption="Jablonec a kopec Kmet" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J11.jpg" caption="Severní pohled na Jablonec" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J12.jpg" caption="Kostel ve večeních hodinách" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J13.jpg" caption="Náves v deštivém počasí" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J14.jpg" caption="Západní pohled na náves" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J15.jpg" caption="Jablonec v zimních měsících" max_width="300px" align="center" %}
<br>
{% include image.html url="images/J17.jpg" caption="Jablonec seshora" max_width="300px" align="center" %}
<br><br>
<h3> Porovnání dobových fotek s 3D modelem </h3>
Kliknutím se změní fotografie na dobovou fotografii
<br>

<img alt="Street"  src="images/J2.jpg" id = "imgClickAndChange" />

<script>     
var images = ["images/J2.jpg", "images/J2O.JPG"]
var imgState = 0;
var imgTag = document.getElementById("imgClickAndChange");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images[imgState];
});

</script> 

<br>
    <img alt="Townhall" src="images/J9.jpg"  id="imgClickAndChange2"   />
    
<script>     
var images2 = ["images/J9.jpg", "images/J9O.JPG"]
var imgState = 0;
var imgTag = document.getElementById("imgClickAndChange2");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images2[imgState];
});

</script> 

<br>

<img alt="Square2" src="images/J8.jpg"  id="imgClickAndChange3"   />

<script>     
var images3 = ["images/J8.jpg", "images/J8O.JPG"]
var imgState = 0;
var imgTag = document.getElementById("imgClickAndChange3");

imgTag.addEventListener("click", function (event) {
  imgState = (++imgState % images.length);
  event.target.src = images3[imgState];
});

</script> 

<h3> Video </h3>
<h5>Video zachycují průlet celou vesnicí Jablonec</h5>

<iframe width="560" height="315" src="https://www.youtube.com/embed/yBfG8Soaxw4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>