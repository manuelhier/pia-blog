---
layout: page 
title: Blog
published: true
---

Hier findest du alle Beiträge in chronologischer Reihenfolge.

---

<ul class="post-list">
  {%- for post in site.posts -%}
    <li>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="post-meta">{{ post.date | date: "%d.%m.%Y" }}</p>
      {% if post.description %}
        <p>{{ post.description }}</p>
      {% else %}
        <p>{{ post.excerpt | strip_html | truncate: 160 }}</p>
      {% endif %}
    </li>
  {%- endfor -%}
</ul>
