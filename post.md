---
layout: main
title: Posts
permalink: /posts/
---

{% for post in site.posts %}
  <h3><a href="/me{{ post.url }}"><strong>{{ post.title }}</strong></a> - {{ post.date | date: "%B %d, %Y" }}</h3>
  <p class="date"></p>
{% endfor %}