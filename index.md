---
layout: default
title: "Articles"
---

# Articles

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.date | date: "%B %d, %Y" }}</p>
      {% if post.thumbnail %}
        <img src="{{ post.thumbnail }}" alt="{{ post.title }} thumbnail">
      {% endif %}
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
