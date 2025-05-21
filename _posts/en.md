---
layout: page
title: Texts in English
permalink: /blog/en/
lang: en  # Use "en" ou "es" para outros idiomas
---

{% raw %}
{% assign posts_en = site.posts | where: "lang", "en" %}
{% for post in posts_en %}
  <h5><a href="{{ post.url }}">{{ post.title }}</a></h5>
  <p>{{ post.date | date: "%d/%m/%Y" }}</p>
{% endfor %}
{% endraw %}
