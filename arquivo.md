---
layout: default
---

<div class="page"> 
<h1 class="orange">timeline{}</h1>

<ul class="taxonomy__index">
  {% assign postsInYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
  {% for year in postsInYear %}
  <h4>
    <a href="#{{ year.name }}">
        <strong>{{ year.name }}</strong> <span class="taxonomy__count">({{ year.items | size }})</span>
    </a>
  </h4>
  {% endfor %}
</ul>
<hr/> <!-- margin-top and margin-bottom in main.css -->
{% for post in site.posts %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}
          </ul>
          <a href="#top" class="btn btn-default" style="font-size: 15px; padding: 0px 5px; margin-left: 30px">
          <span class="fa fa-refresh" aria-hidden="true"></span> Voltar ao início
          </a> 
          {% endunless %}
           <h2 id="{{ currentDate }}"> {{ currentDate }}</h2> <!-- I added new class -->
           <ul>
            {% assign myDate = currentDate %}
            {% endif %}
          <li>
          <a href="{{ post.url }}">{{ post.title }}</a>
          <small class="post-meta" style="color: #313131;"> - Posted on {{ post.date | date: "%B %-d, %Y" }}</small>
        </li>
       {% if forloop.last %}
      </ul>
      {% endif %}
   {% endfor %}
   <a href="#top" class="btn btn-default" style="font-size: 15px; padding: 0px 5px; margin-left: 30px">
      <span class="fa fa-refresh" aria-hidden="true"></span> Voltar ao início
      </a> 
    <hr/>
</div>