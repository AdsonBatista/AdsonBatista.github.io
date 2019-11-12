---
layout: default
title: Sobre mim
permalink: /about/
---
<img src="https://adsonbatista.github.io/images/posts/vida.png"> 

<div id="home">
  <ul class="posts">
    {% for post in site.categories.Vida %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>
</div>
