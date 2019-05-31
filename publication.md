---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please do not
hesitate to <a href="mailto:{{site.email}}">contact me</a>.

{% assign papers_by_year = site.publications | group_by:'year' %}
{% assign papers_by_sorted_year = papers_by_year | sort: 'name' | reverse %}
{% for year in papers_by_sorted_year %}
  <h3>{{ year.name }}</h3>
  <ul>
    {% for paper in year.items %}
    {% assign authors = site.data.authors[paper.authors] %}
    <li>
      <a href="{{ paper.url }}">
        {{ paper.title }} <br>
        {% for author in authors %}
          {{ author.first }} {{ author.last }}
        {% endfor %}
      </a>
    </li>
    {% endfor %}
  </ul><br>
{% endfor %}
