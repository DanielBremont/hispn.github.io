---
layout: page
title: Categorias
---

<p class="message">
  Se puede dejar de lado la identidad nacional es un sistema politico, y en vez defender el bienestar comun,
  sin tocar la identidad.
</p>

**Post :** {{site.posts | size}}

{% for cat in site.categories %}
  <h2 id="{{ cat[0] }}">{{ cat[0] }} ({{ cat[1].size }})</h2>
  <ul>
    
    {% for post in cat[1] reversed %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}

  </ul>
{% endfor %}

<!-- 
{% for tags in site.tags %}
  <h3 id="{{ tags[0] }}">{{ tags[0] }}</h3>
  <ul>
    {% for post in tags[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %} -->