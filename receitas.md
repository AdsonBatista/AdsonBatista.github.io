---
layout: page
title: Receitas
---


Cozinhar é uma arte, uma arte da qual eu gosto de apreciar e de me arriscar as vezes, infelizmente não me considero um bom artista, mas assumo que não dedico parte relevante dos meus esforços no estudo e treinamento desta arte mas, as vezes me arrisco um pouco na cozinha com amigos ou sozinho.

Com intuito de arquivar momentos e receitas utilizarei esta página como um caderno de receitas, onde colocarei cada uma das receitas e variações das mesmas.

<div id="home">
  <ul class="posts">
    {% for post in site.tags.Acompanhamento %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>

  <ul class="posts">
    {% for post in site.tags.Lanche %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>

  <ul class="posts">
    {% for post in site.tags.Bolo %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>


</div>
