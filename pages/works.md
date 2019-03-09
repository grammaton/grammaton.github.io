---
layout: default
title: "WORKS"
subtitle:
description: "vivere è stare svegli. (A. M. Ripellino)"
permalink: /works/
---

## Music for instruments and electronics

<ul class="post-list">
  {% for post in site.categories.mixed %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y" }}</span>
      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <span class="post-meta">{{ post.excerpt | excerpt }}</span>
    </li>
  {% endfor %}
</ul>

## Acousmatic

<ul class="post-list">
  {% for post in site.categories.acousmatic %}
    <li>
      <span class="post-meta">{{ post.date | date: "%Y" }}</span>
      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
      <span class="post-meta">{{ post.excerpt | excerpt }}</span>
    </li>
  {% endfor %}
</ul>
