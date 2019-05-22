---
layout: default
---

<section class="archive-post-list">

{% assign currentDate = post.date | date: "%Y"  %}
    <div class="items">
    {% for post in site.posts %}
    <a href="#{{ currentDate[0] | slugify }}"> <!-- style="color: #1C1C1C;" is font color of cloud index -->
    <div class="item">
      <span> <!-- I get rid of left option -->
        {{ currentDate[0] }} <i><sub>[{{ currentDate | last | size }}]</sub></i>
      </span>
      </div>
    </a>
    {% endfor %}
    </div>
 <!--  </div>-->
  <hr/> <!-- margin-top and margin-bottom in main.css -->

   {% for post in site.posts %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <h1>{{ currentDate }}</h1>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
       <li><a href="{{ post.url }}"><span>{{ post.date | date: "%B %-d, %Y" }}</span> - {{ post.title }}</a></li>
       {% if forloop.last %}</ul>{% endif %}
   {% endfor %}

</section>