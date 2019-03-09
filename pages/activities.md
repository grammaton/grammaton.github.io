---
layout: default
permalink: /activities/
---

## Activities

<!-- <ul class="post-list">
  {% for post in site.categories.activity %}
    <li>{{ post.date | date: "%b %-d, %Y" }} • <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></li>
  {% endfor %}
</ul> -->

<table>
  <tr>
    <th>Date</th>
    <th>Activity</th>
  </tr>
  {% for post in site.categories.activity %}
  <tr>
    <td>{{ post.date | date: "%b %-d, %Y" }}</td>
    <td><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <br> @ {{ post.place }}
        <br> {{ post.excerpt | escape }}
    </td>
  </tr>
  {% endfor %}
</table>
