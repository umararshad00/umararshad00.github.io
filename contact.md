---
layout: page
title: Contact Us
permalink: /contact/
kicker: Contact
subtitle: "The easiest way to reach me is by email."
description: "Contact page for Umar Arshad."
---

<div class="contact-stack">
  <section class="contact-card">
    <h2>Direct contact</h2>
    <p>If you would like to discuss a project, connect for academic collaboration, or simply get in touch, the easiest way to reach me is through email.</p>
    <p>
      <a class="button-primary" href="mailto:{{ site.email }}">{{ site.email }}</a>
    </p>
  </section>

  <section class="contact-grid">
    <div>
      <h3>Email</h3>
      <p><a href="mailto:{{ site.email }}">{{ site.email }}</a></p>
    </div>
    <div>
      <h3>GitHub</h3>
      <p><a href="{{ site.github_url }}">github.com/umararshad00</a></p>
    </div>
    <div>
      <h3>Location</h3>
      <p>{{ site.location }}</p>
    </div>
  </section>
</div>
