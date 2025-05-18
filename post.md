---
layout: main
title: Posts
permalink: /feed/
---

<ul>
  {% for post in site.posts %}
  <li>
    <h3><a href="{{ post.url }}"><strong>{{ post.title }}</strong></a> - {{ post.date | date: "%B %d, %Y" }}</h3>
    <p class="date"></p>
    <p>
    {% if post.tags.size > 0 %}
      {% for tag in post.tags %}
        <strong>{{ tag }}</strong>
        {% unless forloop.last %}, {% endunless %}
      {% endfor %}
    {% endif %}
  </li>
  {% endfor %}
</ul>