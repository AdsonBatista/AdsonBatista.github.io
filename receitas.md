---
layout: default
title: Receitas
permalink: /receitas/
---
<div id="home">

<h1>Categories</h1>
{% for category in site.categories %}

        <a href="{{base_url}}/categories/{{ category | first}}/">
            {{ category | first }}
        </a>
        {% unless forloop.last %}, {% endunless %}

{% endfor %}
<h1>Tags</h1>
<div class="tagcloud">
{% for tag in site.tags %}

    <li style="font-size: {{ tag | last | size | times: 100 | divided_by: site.tags.size| plus: 70 }}%">
        <a href="{{base_url}}/tags/{{ tag | first |downcase | slugize }}/">
            {{ tag | first }}
        </a>

    </li>
{% endfor %}


<img src="https://adsonbatista.github.io/images/posts/comida.png"> 

<div class="tags">Tags: {% for tag in post.tags %}
<a href="{{base_url}}/tags/{{ tag |downcase | slugize }}/">{{tag}}</a>
  {% unless forloop.last %}, {% endunless %}
{% endfor %}</div>

1

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
    {% for post in site.tags.Carne %}
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

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

</div>