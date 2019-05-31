---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please feel free to contact me.

<ul>
  {% for paper in site.publications %}
  <li>
    <a href="{{ paper.url }}">
      {{ paper.title }}
    </a>
  </li>
  {% endfor %}
</ul>
