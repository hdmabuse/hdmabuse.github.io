---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page  # Usa o layout "home" (depende do tema, como "minima" ou customizado)
title: "encruzilhada"  # Título da página
permalink: /pt  # Define a URL da homepage (geralmente "/")
lang: pt
---

## Posts em Português (PT)
{% assign posts_pt = site.posts | where: "lang", "pt" %}
{% if posts_pt.size > 0 %}
  {% for post in posts_pt %}
  - [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
  {% endfor %}
{% else %}
  *Nenhum post em português ainda.*
{% endif %}

