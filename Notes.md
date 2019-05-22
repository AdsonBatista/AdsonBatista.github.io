---
layout: default
title: notes{study}
permalink: /notes/
---

<div id="page">
  <h1 class="orange">notes{study}</h1>
{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
{% assign zz = tag[1] | where: "categories", "Estudos" | sort %}
{% if zz != empty %}

<li><span class="tag">{{ tag[0] }}</span>
<ul>
  {% for p in zz %}
  <li><a href="{{ p.url }}">{{ p.title }}</a></li>
  {% endfor %}
 </ul>
 </li>
 {% endif %}

 {% endfor %}
</div>
