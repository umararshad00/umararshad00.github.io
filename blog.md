---
layout: page
title: "Blog"
permalink: /blog/
description: "University journey, academic reflections, and technical learning notes by Umar Arshad."
subtitle: "Personal reflections, semester experiences, and technical learning notes."
---

This section collects my academic reflections, semester experiences, project work, and practical learning in programming, machine learning, and database systems.

<section class="post-list">
  {% for post in site.posts %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <strong>{{ post.title }}</strong>
    {% if post.subtitle %}
    <span>{{ post.subtitle }}</span>
    {% endif %}
  </a>
  {% endfor %}
</section>
