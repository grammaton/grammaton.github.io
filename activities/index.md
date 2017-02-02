---
layout: page
title: ACTIVITIES
subtitle: "All"
description: "Professional & Artistic Activities"
permalink: /allactivities/
---

<ul class="post-list">
  {% for post in site.categories.activity %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>
