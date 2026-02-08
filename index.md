---
layout: default
title: Home
---

<section class="hero panel">
  <div class="hero-grid">
    <div>
      <h1>Zach Goebel</h1>
      <p class="hero-sub">
        I build thoughtful projects across food, publishing, music, and systems.
      </p>
      <a class="button" href="/contact">Email me</a>
    </div>

    <div>
      {% include margin-note.html text="This site is an experiment — part notebook, part studio log." %}
    </div>
  </div>
</section>

<section class="panel">
  <h2>Selected Projects</h2>
  <p class="section-intro">
    A mix of finished work, ongoing experiments, and ideas in progress.
  </p>

  <div class="project-preview">
    <div class="project-image"></div>
    <div>
      <h3>Towpath Publishing</h3>
      <p>An independent imprint focused on American stories.</p>
      <p class="meta">Publishing · 2024–present</p>
      <a href="https://towpathpublishing.com" target="_blank">Visit site →</a>
    </div>
  </div>

  <div class="project-preview">
    <div class="project-image"></div>
    <div>
      <h3>HobbyADD</h3>
      <p>Explorations in signal craft, creativity, and disciplined curiosity.</p>
      <p class="meta">Media · Ongoing</p>
      <a href="#">Explore →</a>
    </div>
  </div>

</section>

<section class="panel">
  <h2>Recent Writing</h2>

  {% for post in site.posts limit:2 %}
    <div class="writing-preview">
      <p class="meta">{{ post.date | date: "%B %Y" }}</p>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    </div>
  {% endfor %}
</section>
