---
layout: post
title: "Campus Albertov"
image: /images/School_resized.jpg
images:
  - image_path: /images/1.jpg
    title: Apple Pie
  - image_path: /images/2.jpg
    title: Birthday Cake
  - image_path: /images/3.jpg
    title: Black Forest

---


This is visualization of Campus Albertov

<ul class="2016-02-08-Chewbaca-is-talking-in-his-sleep">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
  {% endfor %}
</ul>