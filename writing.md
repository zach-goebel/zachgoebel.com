---
layout: default
title: Writing
---

<section class="panel">
  <h1>Writing</h1>

  {% include margin-note.html text="Most pieces are short (5–10 min). Longer essays are marked with ★." %}

  {% for post in site.posts %}
    <div class="writing-item">
      <p class="meta">{{ post.date | date: "%B %Y" }}</p>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
      <a href="{{ post.url }}">Read more →</a>
    </div>
  {% endfor %}
</section>
