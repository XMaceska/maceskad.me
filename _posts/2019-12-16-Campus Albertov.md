---
layout: post
title: "Campus Albertov"
image: /images/School_resized.jpg
categories: SketchUp,Lumion 9
images:
  - image_path: /images/1.jpg
    title: Purkynuv ustav
  - image_path: /images/2.jpg
    title: Albertov
  - image_path: /images/3.jpg
    title: Purkynuv ustav2
  - image_path: /images/4.jpg
    title: Purkynuv ustav
  - image_path: /images/5.jpg
    title: Albertov
  - image_path: /images/6.jpg
    title: Purkynuv ustav2
  - image_path: /images/7.jpg
    title: Purkynuv ustav
  - image_path: /images/8.jpg
    title: Albertov
  - image_path: /images/9.jpg
    title: Purkynuv ustav2

---


This is visualization of Campus Albertov

<ul class="2019-12-16-Campus Albertov">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
    <br>
  {% endfor %}
</ul>