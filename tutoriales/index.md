---
layout: default
title: Tutoriales
---

<div class="page-header">
  <h1>Tutoriales 🔧</h1>
  <p>Guías paso a paso sobre herramientas, configuraciones y laboratorios.</p>
</div>

<div class="posts-list">
  {% assign tutoriales = site.posts | where: "category", "tutoriales" %}
  {% for post in tutoriales %}
  <a href="{{ post.url | relative_url }}" class="post-item">
    <span class="post-item-title">{{ post.title }}</span>
    <span class="post-item-meta">{{ post.date | date: "%d/%m/%Y" }}</span>
  </a>
  {% endfor %}
  {% if tutoriales.size == 0 %}
  <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
  {% endif %}
</div>
