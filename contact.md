---
layout: page
title: Contact
permalink: /contact
---
{% assign c = site.data.contact %}
<p>Email: <a href="mailto:{{ c.email }}">{{ c.email }}</a></p>
<p>Location: {{ c.location }}</p>
<ul>
  {% for l in c.links %}
    <li><a href="{{ l.url }}" target="_blank">{{ l.label }}</a></li>
  {% endfor %}
</ul>