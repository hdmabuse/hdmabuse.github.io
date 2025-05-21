---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home  # Usa o layout "home" (depende do tema, como "minima" ou customizado)
title: "encruzilhada"  # Título da página
permalink: /  # Define a URL da homepage (geralmente "/")
lang: pt
---

## Posts em Português (PT)
 <ul>
  {% for post in site.posts %}
   {% if post.lang == "pt" %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%d/%m/%Y" }}
      </li>
    {% endif %}
  {% endfor %}
</ul>

## Posts em Inglês (EN)
{% assign posts_en = site.posts | where: "lang", "en" %}
{% if posts_en.size > 0 %}
  {% for post in posts_en %}
  - [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%m/%d/%Y" }})
  {% endfor %}
{% else %}
  *No English posts yet.*
{% endif %}


## Posts em Espanhol (ES)
{% assign posts_es = site.posts | where: "lang", "es" %}
{% if posts_es.size > 0 %}
  {% for post in posts_es %}
  - [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
  {% endfor %}
{% else %}
  *Aún no hay posts en español.*
{% endif %}
{% raw %}
