---
layout: page
title: Posts
orden: 4
---

<ul>
{% for cat in site.categories %}
<li>
  <a href="#{{ cat[0] }}"> {{ cat[0] }} ({{ cat[1].size }})</a>
  </li>
{% endfor %}
</ul>

{% for cat in site.categories %}
  <h2 id="{{ cat[0] }}">{{ cat[0] }} </h2>
  <ul>
    
    {% for post in cat[1] reversed %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}

  </ul>
{% endfor %}