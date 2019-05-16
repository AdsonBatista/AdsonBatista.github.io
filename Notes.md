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


 {% for category in page.categories %}
  {% assign moreThanOneInCategory = false %}
  {% assign posts = site.categories[category] %}

  {% for post in posts %}
    {% if forloop.length > 1 %}
      {% assign moreThanOneInCategory = true %}
    {% endif %}
  {% endfor %}

  {% if moreThanOneInCategory == true %}
    <div class="related-posts">
      <h3>Other posts archived in “{{ category }}”</h3>

      <ul>
        {% for post in posts %}
          {% unless post.url == page.url %}
            <li>
              <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>

              Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
            </li>
          {% endunless %}
        {% endfor %}
      </ul>
    </div>
  {% endif %}
{% endfor %}
</div>
