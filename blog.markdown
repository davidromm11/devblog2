---
layout: default
title: All Posts
permalink: /blog/
---

# All Posts

<div style="display: flex; flex-wrap: wrap; gap: 20px;">

{% for post in site.posts %}
  <div style="flex: 1 1 calc(33% - 20px); box-sizing: border-box; border: 1px solid #ddd; padding: 10px; border-radius: 6px;">
    <a href="{{ post.url }}">
      <h2>{{ post.title }}</h2>
      {% if post.image %}
      <img src="{{ post.image }}" alt="{{ post.title }}" style="max-width: 100%; height: auto; border-radius: 4px;">
      {% endif %}
    </a>
  </div>
{% endfor %}

</div>

