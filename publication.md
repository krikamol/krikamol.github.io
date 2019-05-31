---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please feel free to contact me.

<ul>
  {% for paper in site.categories.papers %}
  <li>
    {{ paper.title }}
  </li>
  {% endfor %}
</ul>
