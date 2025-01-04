---
layout: page
title: Portfolio
permalink: /portfolio/
---

## Selected Portfolio

Here's a selection of projects I've been involved in:

{% for item in site.data.portfolio %}
<hr>

<h3>{{ item.name }}</h3>

<img src="../assets/portfolio/{{ item.name }}.jpg" class="rounded" alt="Album cover art for {{ item.name }}" height="250px" width="250px">

<ul style="list-style: none; margin-left: 0;">
<i>{{ item.role }}</i>
<br>

Released by {{ item.label }} on {{ item.date }}

<li><a href="{{ item.url }}">{% include icons/link.html %} Listen to <i>{{ item.name }}</i></a></li>

<p class="text-muted"><i>{{ item.notes }}</i></p>
</ul>
{% endfor %}