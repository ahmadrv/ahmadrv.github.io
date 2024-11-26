---
layout: default
title: Blog
link: /blog/
---

{% for post in site.posts %}

  <section>
    <a href="{{ post.url }}">
      <h1>{{ post.title }}</h1>
    </a>
    <h2>{{ post.summary }}</h2>
    {{ post.date | date_to_string }}
  </section>

{% endfor %}
