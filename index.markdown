---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---
# Welcome to my site

{% for post in site.posts limit:3 %}
## [{{ post.title }}]({{ post.url }})

{% if post.image %}
![{{ post.title }}]({{ post.image }})
{% endif %}

{{ post.content | strip_html | truncatewords: 50 }}... [read more]({{ post.url }})

---

{% endfor %}

[View all posts](/blog)

