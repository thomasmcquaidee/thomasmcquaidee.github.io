---
layout: page
title: Links
permalink: /links/
---
<h1>Links</h1>
---

links n cool stuff

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
