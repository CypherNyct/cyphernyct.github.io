---
layout: default
title: Writeups
---

<div class="page-header">
  <h1>Writeups 🏴</h1>
  <p>Resolución de máquinas CTF paso a paso.</p>
</div>

<div class="platform-section">
  <h2 class="platform-title">DockerLabs</h2>
  <div class="posts-list">
    {% assign dockerlabs = site.posts | where: "platform", "DockerLabs" %}
    {% for post in dockerlabs %}
    <a href="{{ post.url | relative_url }}" class="post-item">
      <span class="post-item-title">{{ post.title }}</span>
      <span class="post-item-meta">{{ post.difficulty }} · {{ post.date | date: "%d/%m/%Y" }}</span>
    </a>
    {% endfor %}
    {% if dockerlabs.size == 0 %}
    <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
    {% endif %}
  </div>
</div>

<div class="platform-section">
  <h2 class="platform-title">HackTheBox</h2>
  <div class="posts-list">
    {% assign htb = site.posts | where: "platform", "HackTheBox" %}
    {% for post in htb %}
    <a href="{{ post.url | relative_url }}" class="post-item">
      <span class="post-item-title">{{ post.title }}</span>
      <span class="post-item-meta">{{ post.difficulty }} · {{ post.date | date: "%d/%m/%Y" }}</span>
    </a>
    {% endfor %}
    {% if htb.size == 0 %}
    <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
    {% endif %}
  </div>
</div>

<div class="platform-section">
  <h2 class="platform-title">TryHackMe</h2>
  <div class="posts-list">
    {% assign thm = site.posts | where: "platform", "TryHackMe" %}
    {% for post in thm %}
    <a href="{{ post.url | relative_url }}" class="post-item">
      <span class="post-item-title">{{ post.title }}</span>
      <span class="post-item-meta">{{ post.difficulty }} · {{ post.date | date: "%d/%m/%Y" }}</span>
    </a>
    {% endfor %}
    {% if thm.size == 0 %}
    <p style="color: var(--text-muted); font-size: 0.9rem;">Próximamente...</p>
    {% endif %}
  </div>
</div>
