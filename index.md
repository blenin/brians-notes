---
layout: default
title: Inicio
---

<div class="hero">
  <h1>Tecnología e ideas, explicadas sin humo.</h1>
  <p>Escribo para pensar mejor. Sin prisa, sin ruido: una nota a la vez.</p>
</div>

<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <p class="date">{{ post.date | date: "%-d de %B de %Y" }}</p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {% if post.excerpt %}<p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>{% endif %}
  </li>
  {% endfor %}
</ul>
