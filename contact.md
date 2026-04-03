---
layout: page
title: Contact Us
permalink: /contact/
kicker: Get in touch
subtitle: "The easiest way to reach me is by email."
description: "Contact page for Umar Rajput."
---

<div class="contact-stack">
  <section class="contact-callout">
    <h2>Let's connect</h2>
    <p>If you would like to discuss a project, share an opportunity, or simply get in touch, you can contact me directly through email.</p>
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
