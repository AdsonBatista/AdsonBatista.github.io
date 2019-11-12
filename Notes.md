---
layout: default
title: Estudos
permalink: /notes/
---

<div id="page">

<img src="https://adsonbatista.github.io/images/posts/estudos.png"> 

{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
{% assign zz = tag[1] | where: "categories", "Estudos" | sort %}
{% if zz != empty %}


<!--Python
<li><span class="tag">{{ tag[0] }}</span>
-->
<li><span class="tag">{{ Python }}</span>
<ul>
  {% for p in zz %}
  <li><a href="{{ p.url }}">{{ p.title }}</a></li>
  {% endfor %}
 </ul>
 </li>
 {% endif %}

 {% endfor %}
</div>
