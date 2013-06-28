---
layout: index
title: wlrs -- a Jekyll theme
description: "A responsive Jekyll theme."
tags: [Jekyll, theme, responsive, blog, template]
---

  <p>
    <h2>Posts </h2>
    <ul class="posts">
      {% for post in site.posts %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </p>

  <p>
    <h2>Pages </h2>
    <ol class="posts">
      {% for page in site.pages %}
        <li><span> &raquo; </span><a href="{{ site.url }}{{ page.url }}">{{ page.title }}</a></li>
      {% endfor %}
    </ol>
  </p>