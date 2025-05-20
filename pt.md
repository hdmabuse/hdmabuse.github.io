---
layout: page
title: Textos em Português
permalink: /blog/pt/
---

{% raw %}
{% assign posts_pt = site.posts | where: "lang", "pt" %}
{% for post in posts_pt %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date: "%d/%m/%Y" }}</p>
{% endfor %}
{% endraw %}
