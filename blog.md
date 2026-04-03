---
layout: page
title: "Blog"
permalink: /blog/
description: "University journey, academic reflections, and technical learning notes by Umar Arshad."
subtitle: "Personal reflections, semester experiences, and technical learning notes."
nav-menu: true
show_tile: true
image: assets/images/pic03.jpg
---

This section collects my academic reflections, semester experiences, project work, and practical learning in programming, machine learning, and database systems.

<section class="archive-grid">
  {% for post in site.posts %}
  <article class="archive-item">
    <header>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    </header>
    {% if post.subtitle %}
    <p class="meta-intro">{{ post.subtitle }}</p>
    {% endif %}
    {% if post.points %}
    <ul class="summary-points">
      {% for point in post.points limit: 3 %}
      <li>{{ point }}</li>
      {% endfor %}
    </ul>
    {% endif %}
    <ul class="actions">
      <li><a href="{{ post.url | relative_url }}" class="button small">Read Post</a></li>
    </ul>
  </article>
  {% endfor %}
</section>
