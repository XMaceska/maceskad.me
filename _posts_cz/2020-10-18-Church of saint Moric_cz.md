---
layout: post
title: Kostel sv. Mouřence
image: /images/Moric_resized.jpg
SW: "3ds Max 2020"
finished: not yet
lang: cz
ref: moric

---

Jedná se o 3D model kostelu Sv. Mouřence, který se nachází na Šumavě poblíž Kašperských Hor. Tento projekt je tvořen pro G4D. 

Nejprve musím říci, že 3D model jsem dostal v Revitu od G4D a mým cílem bylo vytvořit vizualizaci, ale zároveň umístit kostel na reálné místo za pomocí rozšířené reality. 

[Původní model](https://myhub.autodesk360.com/ue2a46f28/g/shares/SH919a0QTf3c32634dcf9220b99a011d2571?fbclid=IwAR2jE7ycaLDM8OqquhtSV_9YNHdYd2qmUKgAStIRJ8iL8kjGzvYezOy0qQs) byl vytvořen v Revitu se všemi BIM informacemi. Pro mojí práci BIM informace nebyly potřebné a tudíž jsem je ve vizualizaci vůbec nepoužil - převodem do 3ds Maxu jsem o ně i záměrně přišel. Použil jsem pouze polygony modelu. Kompletní vizualizace byla tvořena v 3ds Maxu. Nejprve jsem musel otexturovat model. Zabralo to dost času, ale nakonec se to povedlo. V tomto případě jsem měl k dispozici plno kvalitních fotografií reálného objektu. 

Další věcí bylo vytvořit prostředí, světla, povrch a okolí kostela. Vše jsem vytvořil v CADu. Render byl proveden ve VRAYi. 

Modelován byl rovněž interiér kostelu společně se všemi texturami, vybavením a freskami. Při trasování kamery jsem rovněž vytvořil průlet prostředím s animací otevření dvěří - Díky tomuto projektu jsem se naučil jak animovat CAD objekty. 

Nakonec mým cílem bylo vtyvořit projekci kostela v rozšířené realitě. Plán je nahlédnout do interiéru kostela skrze mobilní aplikaci i v době, kdy je kostel zavřený. nejprva jsem zkoušel vytvořet aplikaci pro mobilní tlefony Android, kterou by si potencionální návštěvník musel stáhnout do svého telefonu. Pro toto jsem použil Unity (naučil jsem se díky tomu základy tvorby mobilních aplikací). Fungovalo to poměrně dobře, ALE ne na všecch telefonech (především na těch starších nikoli) také stahování aplikací není příliž pohodlné.

Přišel jsem tedy s nápad vytvořit webovou stránku, kde poběží za pomocí Javascriptu aplikace pro rozšířenou realitu. Funguje to na této [stránce](https://xmaceska.github.io/ARTEST/). Stránka obsahuje i tlčítko na přepínání jednolivých fází modelu. Dle mého názoru to není špatné, ale ani skvělé. Nyní se potýkám s problémem s náhodným uskakováním modelu okolo správné lokace zapříčiněným GPS signálem. Musím vytvořit určité kotvy a celý model ke kotvám "přichytit". - na tomto nyní pracuji. 

Jako bonus jsem vytvořil modely doml, které se na konkrétním místě nacházeli dříve. opět pomocí Github a toolkitu ARKIT je možné zobrazit na webové stránce domy v rozšířené realitě.

<h3> Rendery </h3>
{% include image.html url="images/M1.jpg" caption="Start - velmi jednoduché, ale již s texturami střech" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M2.jpg" caption="Modelace okolí kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M3.jpg" caption="Úprava okolí kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M4.jpg" caption="Kostel z jiné strany" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M5.jpg" caption="Detail kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M6.jpg" caption="Kostel z jiné strany" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M7.jpg" caption="Kostel z jiné strany" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M10.jpg" caption="Interiér kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M11.jpg" caption="Interiér kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M12.jpg" caption="Interiér kostela" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M13.jpg" caption="Webová mobilní aplikace rozšířené reality" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M14.jpg" caption="Webová mobilní aplikace rozšířené reality" max_width="300px" align="center" %}
<br>
{% include image.html url="images/M15.jpg" caption="Webová mobilní aplikace rozšířené reality" max_width="300px" align="center" %}
<br>