---
layout: page
title: Receitas
---


Cozinhar é uma arte, uma arte da qual eu gosto de apreciar e de me arriscar as vezes, infelizmente não me considero um bom artista, mas assumo que não dedico parte relevante dos meus esforços no estudo e treinamento desta arte mas, as vezes me arrisco um pouco na cozinha com amigos ou sozinho.

Com intuito de arquivar momentos e receitas utilizarei esta página como um caderno de receitas, onde colocarei cada uma das receitas e variações das mesmas.

<div id="home">
  <ul class="posts">
    {% for post in site.categories.Receita %}
   {% for tag in tags %} <!-- style="padding-top: 70px;" is used to deal with nav-custom bar -->
      <h2 id="{{ tag[0] | slugify }}"> {{ tag[0] }}  <i><sub>[{{ tag | last | size }}]</sub></i></h2> <!-- I added new class -->
      <ul> <!-- post-subtitle -->
        {% for post in tag[1] %}
          <a href="{{ site.baseurl }}{{ post.url }}">
        <li>
          {{ post.title }}
        <small class="post-meta" style="color: #313131;"> - Posted on {{ post.date | date: "%B %-d, %Y" }}</small>
        </li>
        </a>
        {% endfor %}
      </ul>
        <a href="#top" class="btn btn-default" style="font-size: 15px; padding: 0px 5px; margin-left: 30px">
          <span class="fa fa-refresh" aria-hidden="true"></span> Voltar ao início
        </a> 
        <hr/>
    {% endfor %}
        {% endfor %}
  </ul>
 <p>Curioso <a href="/about" class="orange">Sobre Mim</a>?</p>
<p></p>
</div>