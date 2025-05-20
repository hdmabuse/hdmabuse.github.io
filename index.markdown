---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home  # Usa o layout "home" (depende do tema, como "minima" ou customizado)
title: "h.d.mabuse"  # Título da página
permalink: /  # Define a URL da homepage (geralmente "/")
language: pt
---
\{% raw %}
## Posts em Português (PT)
{% assign posts_pt = site.posts | where: "lang", "pt" %}
{% for post in posts_pt %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
{% endfor %}

## Posts em Inglês (EN)
{% assign posts_en = site.posts | where: "lang", "en" %}
{% for post in posts_en %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
{% endfor %}

## Posts em Espanhol (ES)
{% assign posts_es = site.posts | where: "lang", "es" %}
{% for post in posts_es %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
{% endfor %}
{% endraw %}
