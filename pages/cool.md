---
layout: page
title: Links
permalink: /links/
---

<h1><small>Links</small></h1>

Here's a list of articles and websites that I want to read over later, but probably haven't gotten round to yet. Currently I'm filling these in by hand, but want to try and work out a way to automate it, as a bit of a reading list for myself.

---

{% for item in site.data.cool-things %}
<h2>{{ item.category }}</h2>
<ul style="list-style: none">
{% for link in item.links %}
<li><a href="{{ link.url }}">{% include icons/link.html %} {{ link.title }}</a></li>
<li> • {{ link.comment }}</li>
{% endfor %}
</ul>
{% endfor %}
