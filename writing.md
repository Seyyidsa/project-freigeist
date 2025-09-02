---
layout: page
title: "Writing"
lang: en
permalink: /writing/
---

## Recent Posts

{% for post in site.posts limit: 10 %}
<div class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <p class="post-description">{{ post.excerpt | strip_html | truncate: 200 }}</p>
    <small class="text-[#49739c]">{{ post.date | date: "%B %d, %Y" }}</small>
</div>
{% endfor %}

## All Posts by Category

### Philosophy
{% for post in site.posts %}
{% if post.category == 'Philosophy' %}
<div class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <p class="post-description">{{ post.excerpt | strip_html | truncate: 150 }}</p>
</div>
{% endif %}
{% endfor %}

### Creativity  
{% for post in site.posts %}
{% if post.category == 'Creativity' %}
<div class="post-item">
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <p class="post-description">{{ post.excerpt | strip_html | truncate: 150 }}</p>
</div>
{% endif %}
{% endfor %}