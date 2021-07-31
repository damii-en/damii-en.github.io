---
layout: default
title: About
---
# BONJOUR 

je m'appelle Damien et voici le blog sur mes passions : les pâtes et les pokémons


{% for tag in site.tags %}
  <h2>{{ tag[0] }}</h2>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.date | date: "%Y-%m-%d" }} {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
