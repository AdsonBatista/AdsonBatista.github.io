---
layout: default
title: Receitas
permalink: /receitas/
---
<div id="home">

<img src="https://adsonbatista.github.io/images/posts/comida.png"> 

  <ul class="posts">
    <h3 class="orange">Acompanhamentos</h3>
    {% for post in site.tags.Acompanhamento %}
    {% assign tags = site.tags | sort %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>

<ul class="posts">
  <h3 class="orange">Carne</h3>
    {% for post in site.tags.Carne %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>

<ul class="posts">
  <h3 class="orange">Frango</h3>
    {% for post in site.tags.Frango %}
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

111

{% for post in site.categories.Receita %}
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
{% endfor %}

</div>