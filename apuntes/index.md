---
layout: default
title: Apuntes
---

<div class="page-header">
  <h1>Apuntes 📓</h1>
  <p>Notas de estudio sobre ciberseguridad, redes, Linux y más.</p>
</div>

<div class="posts-list">
  {% assign apuntes = site.posts | where: "category", "apuntes" %}
  {% for post in apuntes %}
  <a href="{{ post.url | relative_url }}" class="post-item">
    <span class="post-item-title">{{ post.title }}</span>
    <span class="post-item-meta">{{ post.date | date: "%d/%m/%Y" }}</span>
  </a>
  {% endfor %}
  {% if apuntes.size == 0 %}
  <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
  {% endif %}
</div>
