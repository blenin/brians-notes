---
layout: default
title: Inicio
---

<div class="hero">
  <h1>Tecnología e ideas.</h1>
  <p>Escribo para pensar mejor. Sin prisa, sin ruido: una nota a la vez.</p>
</div>

<ul class="post-list">
  {% assign months = "enero|febrero|marzo|abril|mayo|junio|julio|agosto|septiembre|octubre|noviembre|diciembre" | split: "|" %}
  {% assign pinned = site.posts | where: "pinned", true | first %}
  {% assign rest = site.posts | where_exp: "p", "p.pinned != true" %}
  {% if pinned %}
  {% assign m = pinned.date | date: "%-m" | minus: 1 %}
  <li>
    <p class="date">{{ pinned.date | date: "%-d" }} de {{ months[m] }} de {{ pinned.date | date: "%Y" }} <span class="pin-badge">📌 Fijado</span></p>
    <h2><a href="{{ pinned.url | relative_url }}">{{ pinned.title }}</a></h2>
    {% if pinned.excerpt %}<p class="excerpt">{{ pinned.excerpt | strip_html | truncate: 160 }}</p>{% endif %}
  </li>
  {% endif %}
  {% for post in rest %}
  <li>
    {% assign m = post.date | date: "%-m" | minus: 1 %}
    <p class="date">{{ post.date | date: "%-d" }} de {{ months[m] }} de {{ post.date | date: "%Y" }}</p>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    {% if post.excerpt %}<p class="excerpt">{{ post.excerpt | strip_html | truncate: 160 }}</p>{% endif %}
  </li>
  {% endfor %}
</ul>
