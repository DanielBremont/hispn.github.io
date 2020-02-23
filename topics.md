---
layout: page
title: Posts by Topic
---
<ul>
{% for tags in site.tags %}
  <li><a href="#{{tags[0]}}">{{ tags[0] }}</a></li>
{% endfor %}
</ul>

<p class="message">
  Topics has to grow.
  Hey there! This page is included as an example. Feel free to customize it for your own use upon downloading. Carry on!
</p>

{% for tags in site.tags %}
  <h3 id="{{ tags[0] }}">{{ tags[0] }}</h3>
  <ul>
    {% for post in tags[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

Thanks for reading!
