---
layout: page
permalink: /profile/index.html
title: About me
tags: [about, Anuj More, execat]

# Use http://fortawesome.github.io/Font-Awesome/icons/ for "icon" field
networks:
  - site:   Facebook
    text:   facebook.com/execat
    link:   "https://facebook.com/execat"
    icon:   icon-facebook
  - site:   Github
    text:   github.com/execat
    link:   "https://github.com/execat"
    icon:   icon-github
  - site:   Google+
    text:   gplus.to/execat
    link:   "https://plus.google.com/u/0/112656332132179915048/posts"
    icon:   icon-google-plus
  - site:   Twitter
    text:   "@execat"
    link:   "https://twitter.com/execat"
    icon:   icon-twitter
---

Hello, I am Anuj More, the creator of this theme. This is my social profile you can connect me through.

<div class="article-author-top">
{% include author-bio.html %}
</div>

<table>
  <tbody>
    <tr>
      <th></th>
      <th>Network</th>
      <th>Link</th>
    </tr>
  {% for f in page.networks %}
    <tr>
      <td><i class="{{ f.icon }}"></i></td>
      <td>{{ f.site }}</td>
      <td><a href="{{ f.link }}">{{ f.text }}</a></td>
    </tr>
  {% endfor %}
  </tbody>
</table>

<h4>Networks:</h4>
<ul>
  {% for f in page.networks %}
    <li>{{ f.site }}: <a href="{{ f.link }}">{{ f.text }}</a></li>
  {% endfor %}
</ul>
