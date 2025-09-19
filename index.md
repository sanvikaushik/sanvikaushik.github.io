---
layout: page
title: Home
permalink: /
---
{% assign p = site.data.profile %}
<p><strong>Hey—I’m {{ p.name }}.</strong> {{ p.tagline }}</p>
<p><a href="{{ site.resume_url | relative_url }}">View my resume</a></p>
