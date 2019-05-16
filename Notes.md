---
layout: default
title: notes{study}
---

<div id="home">
  <h2 class="orange">notes{study}</h2>
{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
{% assign zz = tag[1] | where: "categories", "Estudos" | sort %}
{% if zz != empty %}

<li><span class="tag">{{ tag[0] }}</span>
<ul>
  {% for p in zz %}
  <li><a href="{{ p.url }}">{{ p.title }}</a></li>
  {% endfor %}
 </ul>
 </li>
 {% endif %}

 {% endfor %}
</div>

{% assign tags = site.tags | where: "categories", "Estudos" | sort %}
<div class="items">
    {% for tag in tags %}
    <a href="#{{ tag[0] | slugify }}"> <!-- style="color: #1C1C1C;" is font color of cloud index -->
    <div class="item">
      <span> <!-- I get rid of left option -->
        {{ tag[0] }} <i><sub>[{{ tag | last | size }}]</sub></i>
      </span>
      </div>
    </a>
    {% endfor %}
 
 <!--  </div>-->
  <hr/> <!-- margin-top and margin-bottom in main.css -->
  <!-- <div class="post-preview">--> <!--post-preview -->
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
          <span class="fa fa-refresh" aria-hidden="true"></span> Go back to the top
        </a> 
        <hr/>
    {% endfor %}
  </div>