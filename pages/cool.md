---
layout: page
title: cool things
permalink: /cool/
---

<h1><small>cool things</small></h1>

here's a list of some stuff i think is cool!

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
