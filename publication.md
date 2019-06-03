---
layout: page
title: Publication
dblp: http://www.informatik.uni-trier.de/~ley/db/indices/a-tree/m/Muandet:Krikamol.html
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please do not
hesitate to <a href="mailto:{{site.email}}">contact me</a>.

My bibliographic information is also available on <a href="{{ page.dblp }}">DBLP</a>.

{% assign authors = site.data.authors %}
{% assign venues = site.data.venues %}
{% assign papers_by_year = site.publications | group_by:'year' %}
{% assign papers_by_sorted_year = papers_by_year | sort: 'name' | reverse %}
{% for year in papers_by_sorted_year %}
  <h3>{{ year.name }}</h3>
  <ul>
    {% for paper in year.items %}
    <li>
      <a href="{{ paper.url }}">
        <strong>{{ paper.title }}</strong>
      </a><br>
      {% for idx in paper.authors %}
        {% assign author = authors[idx] %}
        <small>
        <a href="{{ author.website }}" target="_blank">
          {{ author.first }} {{ author.last }}
        </a>
        </small>
        {% unless forloop.last %}-{% endunless %}
      {% endfor %}
      <br>
      <small><i>{{ venues[paper.venue].name }}
      {% if paper.type == journal or paper.type == conference %}
        {%- if venues[paper.venue].short -%}
          ({{venues[paper.venue].short}})
        {%- endif -%}
      {% endif %}
      </i></small>
    </li>
    {% endfor %}
  </ul>
{% endfor %}
