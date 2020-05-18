---
layout: page
title: Posts
orden: 4
---

{% assign categorieSorted =  site.categories | sort %}

<ul>
{% for cat in categorieSorted %}
<li>
  <a href="#{{ cat[0] }}"> {{ cat[0] }} ({{ cat[1].size }})</a>
  </li>
{% endfor %}
</ul>

{% for cat in categorieSorted %}
  <h2 id="{{ cat[0] }}">{{ cat[0] }} </h2>
  <ul>
    {% assign postSorted =  cat[1] | sort : 'title' %}

    {% for post in postSorted %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}

  </ul>
{% endfor %}