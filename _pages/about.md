---
layout: archive
permalink: /about/
title: "About"
author_profile: true
---

I like to ride cycle and ski, one time,  I used to think about changing my jobs to spend at ski resorts during the winter season.
I am working for capital markets, CCP (Central Couty Party), as an Architect of Interface. 

I have considered how to learn python easily anyone and figured out good site. finally, I have made a guide site for codecademy's python language course.
I hope to help everybody.


{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
