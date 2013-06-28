---
layout: index
title: wlrs -- a Jekyll theme
description: "A responsive Jekyll theme."
tags: [Jekyll, theme, responsive, blog, template]
---

  <p>
    <ul class="posts">
      {% for post in site.posts %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
    </ul>
  </p>

