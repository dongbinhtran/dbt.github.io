---
layout: page
title: About
---
This is the DSRD Statistics webpage

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

