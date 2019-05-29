---
layout: default
title: Receitas
permalink: /receitas/
---

<img src="https://adsonbatista.github.io/images/posts/comida.png"> 

<div id="home">
  <ul class="posts">
    <h3 class="orange">Acompanhamentos</h3>
    {% for post in site.tags.Acompanhamento %}
    {% assign tags = site.tags | sort %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>
    
  <ul class="posts">
  <h3 class="orange">Doces</h3>
    {% for post in site.tags.Doce %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>

  <ul class="posts">
      <h3 class="orange">Lanches</h3>
    {% for post in site.tags.Lanche %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>

  <ul class="posts">
      <h3 class="orange">Massas</h3>
    {% for post in site.tags.Massa %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>
</div>
