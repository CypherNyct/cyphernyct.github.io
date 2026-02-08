---
layout: default
title: Cheatsheets
---

<div class="page-header">
  <h1>Cheatsheets ⚡</h1>
  <p>Referencias rápidas para herramientas y técnicas de pentesting.</p>
</div>

<div class="posts-list">
  {% assign cheatsheets = site.posts | where: "category", "cheatsheets" %}
  {% for post in cheatsheets %}
  <a href="{{ post.url | relative_url }}" class="post-item">
    <span class="post-item-title">{{ post.title }}</span>
    <span class="post-item-meta">{{ post.date | date: "%d/%m/%Y" }}</span>
  </a>
  {% endfor %}
  {% if cheatsheets.size == 0 %}
  <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
  {% endif %}
</div>
