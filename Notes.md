---
layout: default
title: notes{study}
---

<div id="home">
  <h2 class="orange">notes{study}</h2>
  <ul class="posts">
    {% for post in site.categories.Estudos %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
 <p>Curious <a href="/about" class="orange">About Me</a>?</p>
<p></p>
</div>
