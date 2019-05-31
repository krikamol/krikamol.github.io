---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please do not
hesitate to <a href="mailto:{{site.email}}">contact me</a>.

{% assign authors = site.data.authors %}
{% assign papers_by_year = site.publications | group_by:'year' %}
{% assign papers_by_sorted_year = papers_by_year | sort: 'name' | reverse %}
{% for year in papers_by_sorted_year %}
  <h3>{{ year.name }}</h3>
  <ul>
    {% for paper in year.items %}
    <li>
      <a href="{{ paper.url }}">
        {{ paper.title }}
      </a><br>
      {% for idx in paper.authors %}
        {{ idx }}
        <a href="{{ authors[idx].website }}">
          {{ authors[idx].first }} {{ authors[idx].first }}
        </a>
      {% endfor %}
    </li>
    {% endfor %}
  </ul><br>
{% endfor %}
