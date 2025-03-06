---
layout: home
title: Home
---

# Welcome to Y2V.World

Exploring the intersection of impact, public policy, Vedanta, and emerging technologies.

<div class="button-container">
  <a href="/blog" class="button">Read the Blog</a>
</div>

## What is Yukti Vijnana?

A pragmatic approach to knowledge and wisdom, inspired by Swami Vivekananda's Vijnana.

<div class="button-container">
  <a href="/yukti-vijnana" class="button">Learn More</a>
</div>

## Latest Posts

{% for post in site.posts limit:3 %}
<div class="post-preview">
  <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
  <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
  <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 35 }}</p>
  <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
</div>
{% endfor %}
