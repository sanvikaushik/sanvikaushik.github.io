---
layout: page
title: Experience
permalink: /experience
---
{% for e in site.data.experience.items %}
  {% include card.html
    title=e.role | append: ' — ' | append: e.company
    meta=e.location | append: ' · ' | append: e.start | append: ' – ' | append: e.end
  %}
  <ul>
  {% for b in e.bullets %}
    <li>{{ b }}</li>
  {% endfor %}
  </ul>
{% endfor %}
