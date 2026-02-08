---
layout: default
title: Blog
---

<div class="page-header">
  <h1>Blog ✍️</h1>
  <p>Reflexiones, experiencias y mi camino en ciberseguridad.</p>
</div>

<div class="posts-list">
  {% assign blog_posts = site.posts | where: "category", "blog" %}
  {% for post in blog_posts %}
  <a href="{{ post.url | relative_url }}" class="post-item">
    <span class="post-item-title">{{ post.title }}</span>
    <span class="post-item-meta">{{ post.date | date: "%d/%m/%Y" }}</span>
  </a>
  {% endfor %}
  {% if blog_posts.size == 0 %}
  <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
  {% endif %}
</div>
