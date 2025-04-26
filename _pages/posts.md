---
title: "Posts"
layout: single
permalink: /posts/
author_profile: true
---

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | truncatewords: 30 }}</p>
  </article>
{% endfor %}