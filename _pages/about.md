---
layout: archive
permalink: /about/
title: "About"
author_profile: true
---

자전거 타는것을 좋아하고,     
겨울내내 스키를 타고 싶어 직업을 바꿔 볼까도 생각했다.    
자본시장관련 금융 인터페이스 아키텍트로 활동하고 있다.    

누구나 쉽게 Python을 배울 방법이 없을까 고민하다,    
좋은 사이트를 알게 되었다.   
결국 이를 공부하는데 도움이 될만한 가이드 사이트를 만들게 되었다.    
도움이 되었으면 좋겠다.


{% include group-by-array collection=site.posts field="categories" %}
{% for category in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ category | slugify }}" class="archive__subtitle">{{ category }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
