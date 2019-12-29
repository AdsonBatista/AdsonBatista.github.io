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



{% assign post = page %}
{% if post.tags.size > 0 %}
  {% capture tags_content %}Posted with {% if post.tags.size == 1 %}<i class="icon icon-tag"></i>{% else %}<i class="icon icon-tags"></i>{% endif %}: {% endcapture %}
  {% for post_tag in post.tags %}
    {% for data_tag in site.data.tags %}
      {% if data_tag.slug == post_tag %}
        {% assign tag = data_tag %}
      {% endif %}
    {% endfor %}
    {% if tag %}
      {% capture tags_content_temp %}{{ tags_content }}<a href="/blog/tag/{{ tag.slug }}/">{{ tag.name }}</a>{% if forloop.last == false %}, {% endif %}{% endcapture %}
      {% assign tags_content = tags_content_temp %}
    {% endif %}
  {% endfor %}
{% else %}
  {% assign tags_content = '' %}
{% endif %}