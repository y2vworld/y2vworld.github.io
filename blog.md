---
layout: page
title: Blog
permalink: /blog/
---

# Blog

Explore our latest thoughts and insights on technology, policy, and Vedantic philosophy.

{% for post in site.posts %}
<div class="post-preview">
  <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
  <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
  <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 35 }}</p>
  <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
</div>
{% endfor %}
