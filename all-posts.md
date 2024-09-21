---
layout: default
title: All Posts
permalink: /all-posts/
---

# All Posts

<ul>
  {% for post in site.posts %}
    <li>
      <h4><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h4>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
