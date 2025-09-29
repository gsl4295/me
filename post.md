---
layout: main
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  <h2><a href="/me{{ post.url }}"><strong>{{ post.title }}</strong></a></h2>
  by <em>{{ post.author }}</em><br>
  {{ post.date | date: "%B %d, %Y" }}
{% endfor %}