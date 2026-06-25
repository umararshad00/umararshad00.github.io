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
{% assign introduction_posts = ordered_posts | where: "blog_category", "introduction" %}
{% assign first_semester_posts = ordered_posts | where: "blog_category", "first-semester" %}
{% assign second_semester_posts = ordered_posts | where: "blog_category", "second-semester" %}
{% if site.posts.size > 0 %}
<section class="blog-category" id="introduction">
  <header class="category-heading">
    <p class="eyebrow">Category</p>
    <h2>Introduction</h2>
    <p>The starting point of my university journey and the first step into academic life.</p>
  </header>
  <div class="blog-list">
    {% for post in introduction_posts %}
      {% include post-card.html %}
    {% endfor %}
  </div>
</section>

<section class="blog-category" id="first-semester">
  <header class="category-heading">
    <p class="eyebrow">Category</p>
    <h2>First Semester</h2>
    <p>Programming fundamentals, machine learning practice, project work, presentations, and final-week progress.</p>
  </header>
  <div class="blog-list">
    {% for post in first_semester_posts %}
      {% include post-card.html %}
    {% endfor %}
  </div>
</section>

<section class="blog-category" id="second-semester">
  <header class="category-heading">
    <p class="eyebrow">Category</p>
    <h2>Second Semester</h2>
    <p>Database systems, WordPress learning, online study adjustments, campus reopening, and midterm preparation.</p>
  </header>
  <div class="blog-list">
    {% for post in second_semester_posts %}
      {% include post-card.html %}
    {% endfor %}
  </div>
</section>
{% else %}
<article class="content-card">
  <p>No posts have been published yet.</p>
</article>
{% endif %}
