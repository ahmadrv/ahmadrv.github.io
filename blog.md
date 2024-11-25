---
layout: default
title: Blog
link: /blog/
---

{% for post in site.posts %}
  <p><a href="{{ post.url }}">{{ post.title }}</a><br>
  {{ post.summary }}<br>
  {{ post.date | date_to_string }}</p>
{% endfor %}