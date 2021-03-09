---
layout: page
title: Students
permalink: /student/
---

<p>I am grateful for all of my students. If you are interested in working with me, I will be glad to hear from you.</p>

{% assign students = site.data.students %}
<ul>
  {% for student in student %}
      {% assign key = author[0] %}
      <li>
      {%- if authors[key].website -%}  
        <a href="{{ authors[key].website }}" target="_blank">
      {%- endif -%}
        {{ authors[key].first }} {{ authors[key].last }}
      {%- if authors[key].website -%}
          </a>
      {%- endif -%}
      {%- if authors[key].affiliation -%}
        &nbsp;({{ authors[key].affiliation }})
      {%- endif -%}
      </li>
  {% endfor %}
</ul>
