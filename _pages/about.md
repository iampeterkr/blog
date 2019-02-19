---
layout: archive
permalink: /about/
title: "About"
author_profile: true
---

I like to ride road cycle and ski.   
One time, I used to consider changing my jobs, in order to go skiing at the ski resorts during winter seasons.
I am working for capital markets, CCP (Central Couty Party), as an Architect of Interface.     


I have considered how to learn python easily anyone and figured out a good site finally. so, make a guide site, "The python grammar guide course of Codecademy", for the beginner programmer and lecture the python grammar Using "Codecademy" sometimes.    
I hope to help everybody.



**From *Wonyoung***

{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
