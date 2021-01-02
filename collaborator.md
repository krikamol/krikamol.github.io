---
layout: page
title: Collaborator
permalink: /collaborator/
---

<p>I am grateful for the following people with whom I collaborated and have collaborated on various projects.  I always seek new collaboration, so I will be glad to hear from you.</p>

{% assign authors = site.data.authors %}
<ul>
{% for author in authors %}
      {% assign col = authors[author[0]] %}
      <li>
      {% if col.website %}  
        <a href="{{ col.website }}" target="_blank">
      {%- endif -%}
        {{ col.first }} {{ col.last }}
      {% if col.website %}  
          </a>
      {%- endif -%}
      {% if col.affiliation %}
        ({{ col.affiliation }})
      {%- endif -%}
      </li>
{% endfor %}
</ul>
