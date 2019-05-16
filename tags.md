---
layout: page
title: Tags
---

<div class="page">
  {% assign sorted_tags = site.data.tags | sort:"name" %}
  {% for tag in sorted_tags %}
    {% include tag_link_formatter.html tag=tag tag_separator='<br />' %}
  {% endfor %}


  {% if site.tags != "" %}
  {% include tag_collector.html %}
{% endif %}
</div>

