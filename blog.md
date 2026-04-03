---
layout: page
title: "Blog"
permalink: /blog/
kicker: Journal
body_class: blog-page
description: "University journey, academic reflections, and technical learning notes by Umar Arshad."
subtitle: "Personal reflections, semester experiences, and technical learning notes."
---

<p>This section collects my academic reflections, semester experiences, project work, and practical learning in programming, machine learning, and database systems.</p>

{% assign ordered_posts = site.posts | sort: "sequence" %}
{% if site.posts.size > 0 %}
<section class="blog-list">
  {% for post in ordered_posts %}
    <article class="post-preview">
      {% if post.image %}
        <a class="post-preview-media" href="{{ post.url | relative_url }}" aria-label="{{ post.title }}">
          <img src="{{ post.image | relative_url }}" alt="{{ post.image_alt | default: post.title }}" loading="lazy">
        </a>
      {% endif %}
      <div class="post-preview-copy">
        {% if post.sequence %}
          <p class="post-sequence">Part {{ post.sequence }}</p>
        {% endif %}
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.subtitle %}
          <p class="post-subtitle">{{ post.subtitle }}</p>
        {% endif %}
        {% if post.image_caption %}
          <p class="post-media-note">{{ post.image_caption }}</p>
        {% endif %}
        {% if post.points %}
          <ul class="compact-points">
            {% for point in post.points limit: 3 %}
              <li>{{ point }}</li>
            {% endfor %}
          </ul>
        {% endif %}
        <a class="text-link" href="{{ post.url | relative_url }}">Read full post</a>
      </div>
    </article>
  {% endfor %}
</section>
{% else %}
<article class="content-card">
  <p>No posts have been published yet.</p>
</article>
{% endif %}
