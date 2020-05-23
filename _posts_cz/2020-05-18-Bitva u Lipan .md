---
layout: post
title: "Bitva u Lipan"
image: /images/lipany_resized.jpg
SW: "3ds Max 2020"
finished: 18.05.2020
lang: cz
ref: lipany

---


V tomto projektu jsem se věnoval vizualizaci schématu bitvy u Lipan. Bitva u Lipan se odehrála v roce 1436 poblíž vesničky Lipany. Na jedné straně stáli radikální husité a na strně druhé umírnění husité. 

Toto byla moje první práce pro firmu G4D. Hlavním účelem této vizualizace bylo jasně a přehledně představit schéma bitvy u lipan ve 3D. Zákazník si objednal tuto práci u G4D za účelem udělat dojem na komisi při obhajobě své diplomové práce. Diplomová práce zákazníka se věnuje bitvě u Lipan a jak víme, tak vše vypadá lépe ve 3D a proto dostal nápad schéma bitvy vizualizovat ve 3D. Nyní tedy přichází řada na mě. 

Celý proces modelace byl pro mně vlastně částečně jiný a nový. Prvně jsem se musel vypořádat s absencí některých softwarů, na které jsem byl dříve zvyklý. Já jakožto student, jsem měl vždy přístup ke všem možným softwarům se studentskou licencí a tak jsem si na všechny tyto komerční SW zvykl. Jenže vlastnit všechny komerční SW se firmě prostě nevyplatí. Tento projekt je už opravdu komerční a proto studentskou verzi použít nemohu a všechny licence musí být ok. Naštěstí G4D vlastní licenci Autodesk konkétně balíček ve, kterém je 3ds Max. Na druhou stranu nevlastní Lumion ani Photoshop (V průběhu jsem zjistil, že Gimp je o několik set km dál svojí funkčností, než Photoshop a konečně jsem se od Photoshopu odprostil a začal naplno používat Gimp. Je fakt super).

Do této chvíle jsem vždy tvořil geometrii v 3ds Maxu a následnou tvorbu materiálů, textur, světel a nastavení renderu jsem dělal v Lumionu. Abych se přiznal dělal jsem to pro ulehčení práce. Nastavení v Lumionu je naprosto jednoduché a intuitivní. Jednou ale ten čas, kdy se od něj budu muset odprostit a naučit se pořádně s 3ds Maxem musel přijít a přišel teď. Ve finále jsem teď za to dost rád. 3ds Max nabízí násobně mnohem dokonalejší možnosti nastavení. Obtížnost je tedy několikanásobně složitější, ale výsledek je násobně lěpší. 

Povrch jsem vytvořil z dodaného DMR 5G, což je digitální model reliéfu ČR vytvořen leteckým laserovým skenováním. Úsek potřebný pro můj projekt pořídila firma G4D a já jsem musel zpracovat data. ČÚZK DMR prodává ve formě XYZ bodů (Několik miliónu bodů byla moje počáteční pozice na tomto projektu). XYZ body jsem tedy musel převést do meshe, abych mohl vůbec začít pracovat.

Následovalo modelování povrchu, především všech potoků, řek a cest, které tam byly dříve a teď už nejsou. Zároveň jsem povrch musel vyhladit, tak aby zmizely nerovnosti typu solární elektrárna, vesničky, které dříve neexistovaly, apod. Musel jsem projít skrze práci jako je vertex paint, odrazy ve vodě, multi-sub textury, nastavení prostředí, mlhy, displacement, bump, apod. Celkově jsem na projektu oficiálně strávil 80 hodin. Ale abych byl upřímný strávil jsem s tím ještě déle zejména z důvodu učení se nových věcí v 3ds Maxu.

Nakonec jsem ještě měl problémy s exportem. Jelikož G4D chtělo celý model v .obj pro prezentaci na jejich webové stránce. Naneštěstí všechny možné textury a materiály byl dost komplexní na to, aby export proběhl hladce a jednoduše. Mnoho nastavení v modelu je čitelné pouze pro 3ds Max a tedy po exportu se se model zobrazoval pouze jako geometrie (ještě ke všemu zdeformovaná) bez textur. Naštěstí jsem se naučil jak "vypéct" textury následně se export povedl. 


<h3> Renders </h3>

Jen pro ujasnění jak probíhala bitva:
1 - Začátku proti sobě stály oba tábory radikálních (modří) a umírněních (červení) husitů.
2 - Následovalo mírný útok (několik salv) radikálů na umírněný husity.
3 - Radikálové následně předstírali ústup a umírnění zaútočili.
4 - radikálové následně vytáhli svojí skrytou zbraň - doslova skrytá kavalérie (modrý obdélník).
5 - umírnění husté se museli stáhnout a jejich základna byla za pomocí kavalérie dobyta.



{% include image.html url="images/44.jpg" caption="1 - tábor radikálů (modrá) a umírněných (červená) husitů" max_width="300px" align="center" %}
<br>
{% include image.html url="images/49.jpg" caption="2 - Radikálové mírně útočí" max_width="300px" align="center" %}
<br>
{% include image.html url="images/50.jpg" caption="3 - Radikálové předstírají ústup" max_width="300px" align="center" %}
<br>
{% include image.html url="images/53.jpg" caption="4 - Radikálové používají kavalérii" max_width="300px" align="center" %}
<br>
{% include image.html url="images/48.jpg" caption="5 - ústup umírněných husitů" max_width="300px" align="center" %}
<br>
{% include image.html url="images/38(1).jpg" caption="Povrch bez schématu" max_width="300px" align="center" %}
<br>
{% include image.html url="images/55.jpg" caption="Povrch bez schématu" max_width="300px" align="center" %}
<br>
{% include image.html url="images/33.jpg" caption="Povrch bez schématu" max_width="300px" align="center" %}
<br>