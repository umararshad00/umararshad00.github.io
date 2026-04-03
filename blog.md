---
layout: default
title: "Blog"
permalink: /blog/
body_class: blog-page
description: "University journey, academic reflections, and technical learning notes by Umar Arshad."
---

{% assign featured = site.posts | first %}

<section class="journal-hero content-card">
  <div>
    <p class="eyebrow">Writing Archive</p>
    <h1>University Journey and Learning Notes</h1>
    <p class="lead">This section collects my academic reflections, semester experiences, project work, and practical learning in programming, machine learning, and database systems.</p>
  </div>
  <div class="stats-row">
    <div class="stat-chip">
      <strong>{{ site.posts | size }}</strong>
      <span>Published posts</span>
    </div>
    <div class="stat-chip">
      <strong>Python, ML, DBMS</strong>
      <span>Core learning </span>
    </div>
    
  </div>
</section>

{% if site.posts.size > 0 %}
  {% if featured %}
  <section class="featured-story">
    <div class="story-copy">
      <p class="eyebrow">Featured Reflection</p>
      <h2><a href="{{ featured.url | relative_url }}">{{ featured.title }}</a></h2>
      <p class="lead">{{ featured.subtitle }}</p>
      <p>{{ featured.excerpt | strip_html | strip_newlines | truncate: 220 }}</p>
      {% if featured.topics %}
      <div class="tag-list">
        {% for topic in featured.topics %}
          <span class="tag-pill">{{ topic }}</span>
        {% endfor %}
      </div>
      {% endif %}
      <a class="button-primary" href="{{ featured.url | relative_url }}">Read featured post</a>
    </div>
    {% if featured.points %}
    <aside class="story-aside">
      <ul class="story-points">
        {% for point in featured.points %}
          <li>{{ point }}</li>
        {% endfor %}
      </ul>
    </aside>
    {% endif %}
  </section>
  {% endif %}

  <section class="section-heading">
    <p class="eyebrow">More Reflections</p>
    <h2>Academic reflections and practical project notes</h2>
  </section>

  <section class="blog-grid rich-blog-grid">
    {% for post in site.posts offset: 1 %}
      <article class="post-preview">
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.subtitle %}
          <p class="post-subtitle">{{ post.subtitle }}</p>
        {% endif %}
        {% if post.points %}
        <ul class="compact-points">
          {% for point in post.points limit: 3 %}
            <li>{{ point }}</li>
          {% endfor %}
        </ul>
        {% endif %}
        {% if post.topics %}
        <div class="tag-list">
          {% for topic in post.topics limit: 3 %}
            <span class="tag-pill">{{ topic }}</span>
          {% endfor %}
        </div>
        {% endif %}
        <a class="text-link" href="{{ post.url | relative_url }}">Read full post</a>
      </article>
    {% endfor %}
  </section>
{% else %}
<article class="content-card">
  <p>No posts have been published yet.</p>
</article>
{% endif %}
