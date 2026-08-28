---
layout: page
title: Blog
permalink: /blog/
description: Blog posts by Congyan (Cruise) Song.
---

{% if site.posts.size > 0 %}
<ul style="list-style:none; padding-left:0;">
{% for post in site.posts %}
  {% if post.external_url %}{% assign href = post.external_url %}{% else %}{% assign href = post.url | relative_url %}{% endif %}
  <li style="margin-bottom:18px;">
    <a href="{{ href }}" style="font-size:1.05rem;"{% if post.external_url %} target="_blank" rel="noopener"{% endif %}>{{ post.title }}</a>{% if post.external_url %} <i class="fa-solid fa-arrow-up-right-from-square" style="font-size:0.75rem; color:#999;"></i>{% endif %}<br>
    <small>{{ post.date | date: "%B %-d, %Y" }}</small>
    {% if post.excerpt and post.external_url == nil %}<div style="margin-top:4px;">{{ post.excerpt }}</div>{% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
<p>No posts yet — check back soon!</p>
{% endif %}
