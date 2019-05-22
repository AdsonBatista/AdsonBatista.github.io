---
layout: default
title: life{me}
permalink: /life/
---

<div id="home">
  <h1 class="orange">life{me}</h1>
  <ul class="posts">
    {% for post in site.categories.Vida %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>
</div>
