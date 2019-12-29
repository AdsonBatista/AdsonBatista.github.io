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

  {% assign page_depth = page.url | split: '/' | size %}
  {% assign page_parent = page.url | split: '/' | last %}
  {% for node in site.pages offset:1 %}
  {% if node.url == '/' %}
  {{ continue }}
  {% else %}
  {% assign split_path = node.url | split: "/" %}
  {% assign node_last = split_path | last %}
  {% assign node_parent = node.url | remove: node_last | split: '/' | last %}
  {% assign node_url = node.url %}
  {% for slug in split_path offset:1 %}
  {% assign slug = slug %}
  {% assign slug_depth = forloop.index %}
  {% endfor %}
  {% if slug_depth == page_depth and page_parent == node_parent %}
  <li><a href="{{ node_url }}">{{ slug }}</a></li>
  {% endif %}
  {% if slug_depth == 1 and page.url == '/' and slug != 'search.json' and   slug != 'sitemap.xml' %}
  <li><a href="{{ node_url }}">{{{slug}}</a></li>
  {% endif %}
  {% endif %}
  {% endfor %}


2

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