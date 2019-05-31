---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please feel free to contact me.

{% assign papers_by_year = site.publications | group_by:'year' %}
{% for year in papers_by_year %}
  <h3>{{ year.name }}</h3>
  <hr>
  <ul>
    {% for paper in year.items %}
    <li>
      <a href="{{ paper.url }}">
        {{ paper.title }}
      </a>
    </li>
    {% endfor %}
  </ul><br>
{% endfor %}
