---
layout: page
title: Projects
permalink: /projects
---
{% for pr in site.data.projects.items %}
  {% include card.html
    title=pr.name
    body=pr.summary
    link=pr.link
  %}
  {% if pr.tags %}
    <p style="margin-top:-.5rem;color:#666;">{{ pr.tags | join: ' · ' }}</p>
  {% endif %}
{% endfor %}
