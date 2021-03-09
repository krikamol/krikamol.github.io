---
layout: page
title: Students
permalink: /student/
---

<p>I am grateful for all of my students. I am really proud of them. If you are interested in working with me, I will be glad to hear from you.</p>

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
        &nbsp;(<i>{{ students[key].title }}</i>, {{ students[key].affiliation }})
      {%- endif -%}
      </li>
  {% endfor %}
</ul>
