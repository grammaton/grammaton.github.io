---
layout: default
permalink: /blog/
---

## Blog

<ul class="post-list">
  {% for post in site.categories.blog %}
    <li>{{ post.date | date: "%b %-d, %Y" }} • <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></li>
  {% endfor %}
</ul>
