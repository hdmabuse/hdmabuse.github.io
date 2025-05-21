---
layout: page
title: Textos en Español
permalink: /blog/es/
---

{% raw %}
{% assign posts_es = site.posts | where: "lang", "es" %}
{% for post in posts_es %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h5>
  <p>{{ post.date | date: "%d/%m/%Y" }}</p>
{% endfor %}
{% endraw %}
