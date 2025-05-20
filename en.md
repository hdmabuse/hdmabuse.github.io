---
layout: page
title: Texts in English
permalink: /blog/en/
---

{% raw %}
{% assign posts_en = site.posts | where: "lang", "en" %}
{% for post in posts_en %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.date | date: "%d/%m/%Y" }}</p>
{% endfor %}
{% endraw %}
