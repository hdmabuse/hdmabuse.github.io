---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

---
# Front matter (metadados obrigatórios para o Jekyll processar a página)
layout: home  # Usa o layout "home" (depende do tema, como "minima" ou customizado)
title: "h.d.mabuse"  # Título da página
permalink: /  # Define a URL da homepage (geralmente "/")
---
# Boas-vindas ao Meu Site! 👋

Olá! Este é meu espaço pessoal para compartilhar ideias, notas do Obsidian e projetos.
Aqui você encontrará:

- 📚 **Artigos** sobre tecnologia, produtividade e aprendizado.
- 🗒️ **Notas públicas** do meu vault do Obsidian.
- 🛠️ Projetos open-source que desenvolvo.

---

## Últimos Posts

{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%d/%m/%Y" }})
{% endfor %}

---

## Sobre Mim

Sou um entusiasta de [insira sua área], e uso este site para documentar meu aprendizado.
📫 Me encontre no:
- GitHub: [@seu-usuario](https://github.com/seu-usuario)
- LinkedIn: [seu-perfil](https://linkedin.com/in/seu-perfil)
