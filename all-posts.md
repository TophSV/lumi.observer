---
layout: default
title: All Posts
permalink: /all-posts/
description: {{ site.description }}
image: /assets/images/lumi_observe_ascii_art.png
---
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "WebSite",
  "name": "{{ site.title }}",
  "url": "{{ site.url }}",
  "description": "{{ site.description }}",
  "author": {
    "@type": "{{ site.author.type }}",
    "name": "{{ site.author.name }}"
  }
}
</script>

# All Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      <p>{{ post.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
