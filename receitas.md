---
layout: page
title: Receitas
---


Cozinhar é uma arte, uma arte da qual eu gosto de apreciar e de me arriscar as vezes, infelizmente não me considero um bom artista, mas assumo que não dedico parte relevante dos meus esforços no estudo e treinamento desta arte mas, as vezes me arrisco um pouco na cozinha com amigos ou sozinho.

Com intuito de arquivar momentos e receitas utilizarei esta página como um caderno de receitas, onde colocarei cada uma das receitas e variações das mesmas.

<div id="home">
  <ul class="posts">
    <h3 class="orange">Acompanhamentos</h3>
    {% for post in site.tags.Acompanhamento %}
    {% assign tags = site.tags | sort %}
      <li><span>{{ post.tag }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>

  <ul class="posts">
      <h3 class="orange">Lanches</h3>
    {% for post in site.tags.Lanche %}
      <li><span>{{ post.tag }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>
    
  <ul class="posts">
  <h3 class="orange">Doces</h3>
    {% for post in site.tags.Doce %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
<p></p>


</div>
