---
layout: page
title: Students
permalink: /student/
---

<p>I am grateful for all of my students. I am really proud of them.</p>

{% assign students = site.data.students %}
<ul>
  {% for student in students %}
      {% assign key = student[0] %}
      <li>
      {%- if students[key].website -%}  
        <a href="{{ students[key].website }}" target="_blank">
      {%- endif -%}
        {{ students[key].first }} {{ students[key].last }}
      {%- if students[key].website -%}
          </a>
      {%- endif -%}
      {%- if students[key].affiliation -%}
	{%- if students[key].status == "finished" -%}
          &nbsp;(<i>{{ students[key].title }}</i>, Now at {{ students[key].affiliation }})
	{%- elsif students[key].status == "active" -%}
          &nbsp;(<i>{{ students[key].title }}</i>, {{ students[key].affiliation }})
	{%- endif -%}
      {%- endif -%}
      </li>
  {% endfor %}
</ul>
