---
layout: page
title: Textos em Português
permalink: /blog/pt/
---

# Posts em Português

<ul>
  {% for post in site.posts %}
    {% if post.lang == "pt" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%d/%m/%Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>
