---
title: "Posts"
layout: single
permalink: /posts/
author_profile: true
---

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <small>{{ post.date | date: "%B %d, %Y" }}</small>
    <p>{{ post.excerpt | strip_html | truncatewords: 15 }}</p>
  </article>
{% endfor %}