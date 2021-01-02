---
layout: page
title: Publication
semantic_scholar: https://www.semanticscholar.org/author/Krikamol-Muandet/2276351
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please do not
hesitate to <a href="mailto:{{site.email}}">contact me</a> directly.


My bibliographic information are also available on <a href="https://scholar.google.com/citations?user={{ site.scholar_username }}" target="_blank">Google Scholar</a>, <a href="https://dblp.uni-trier.de/pers/hd/m/{{ site.dblp_username }}" target="_blank">DBLP</a>, and <a href="{{ page.semantic_scholar }}" target="_blank">Semantic Scholar</a>.


{% assign authors = site.data.authors %}
{% assign venues = site.data.venues %}
{% assign papers_by_year = site.publications | group_by:'year' %}
{% assign papers_by_sorted_year = papers_by_year | sort: 'name' | reverse %}
{% for year in papers_by_sorted_year %}
  <h3>{{ year.name }}</h3>
    <ul>
    {% assign papers_by_sorted_venue = year.items | sort: 'venue' %}
    {% for paper in papers_by_sorted_venue %}
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
      {% if paper.type == "journal" %}
        {%- if venues[paper.venue].short -%}
          ({{venues[paper.venue].short}})
        {%- endif -%}
      {% elsif paper.type == "conference" %}
        {%- if venues[paper.venue].short -%}
          ({{venues[paper.venue].short}} {{paper.year}})
        {%- endif -%}
      {% endif %}
      </i></small>
      {% if paper.remark %}
        <br>
        <small><i>
        <span style="color:red">* {{paper.remark]}}</span>
        </i></small>
        {%- endif -%}
    </li>
    {% endfor %}
  </ul>
{% endfor %}
