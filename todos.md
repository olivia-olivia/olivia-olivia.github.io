---
layout: default
title: todos,
category:
permalink: /todos/
---

começando pelos mais recentes.

<div id="index-posts">
  {% for post in site.posts %}
  <div id="post-short">
    <a href="{{site.url}}{{site.baseurl}}{{post.url}}">
      <h3>{{post.title}}</h3>
    </a>
    <p>
      {% if post.excerpt %}
        {{ post.excerpt }}
      {% else %}
        {{ post.content }}
      {% endif %}
    </p>
  </div>
  {% endfor %}
</div>
