---
layout: default
title: "Blog"
permalink: /blog/
body_class: blog-page
description: "Blog posts and personal experiences by Umar Rajput."
---

<section class="section-heading">
  <p class="eyebrow">Writing</p>
  <h1>Blog</h1>
  <p class="lead">All posts are listed here. Click any title or button to open the full post and read it completely.</p>
</section>

{% if site.posts.size > 0 %}
<section class="blog-grid">
  {% for post in site.posts %}
    <article class="post-preview">
      <p class="post-date">{{ post.date | date: site.date_format }}</p>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt | strip_html | strip_newlines | truncate: 180 }}</p>
      <a class="text-link" href="{{ post.url | relative_url }}">Read full post</a>
    </article>
  {% endfor %}
</section>
{% else %}
<article class="content-card">
  <p>No posts have been published yet.</p>
</article>
{% endif %}
