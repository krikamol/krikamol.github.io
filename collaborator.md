---
layout: page
title: Collaborator
permalink: /collaborator/
---

<p>I am grateful for the following people with whom I collaborated and have collaborated on various projects.  I always seek new collaboration, so I will be glad to hear from you.</p>

{% assign authors = site.data.authors %}
<ul>
  {% for author in authors %}
      {% assign key = author[0] %}
      <li>
      {% if authors[key].website %}  
        <a href="{{ authors[key].website }}" target="_blank">
      {%- endif -%}
        {{ authors[key].first }} {{ authors[key].last }}
      {% if authors[key].website %}  
          </a>
      {%- endif -%}
      {% if authors[key].affiliation %}
        ({{ authors[key].affiliation }})
      {%- endif -%}
      </li>
  {% endfor %}
</ul>
