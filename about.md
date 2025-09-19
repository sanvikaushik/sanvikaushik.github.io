---
layout: page
title: About
permalink: /about
---
{% assign p = site.data.profile %}
<p>{{ p.intro }}</p>

{% if p.photos %}
<div style="display:flex;gap:12px;flex-wrap:wrap;margin-top:1rem;">
  {% for ph in p.photos %}
    <img src="{{ ph | relative_url }}" alt="Sanvi photo {{ forloop.index }}" style="max-width:280px;border-radius:12px;border:1px solid #eee;">
  {% endfor %}
</div>
{% endif %}
