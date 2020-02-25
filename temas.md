---
layout: page
title: Entradas por temas
---

<p class="message">
  Los temas tienen que crecer.
 ¡Hola! Esta página se incluye como ejemplo. Siéntase libre de personalizarlo para su propio   uso al descargarlo. ¡Continua!
</p>

{% for tags in site.tags %}
  <h3 id="{{ tags[0] }}">{{ tags[0] }}</h3>
  <ul>
    {% for post in tags[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
