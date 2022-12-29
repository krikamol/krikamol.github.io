---
layout: page
title: Students
permalink: /student/
---

<p>Here are my past and current brilliant students with whom I have been fortunate to collaborate.</p>

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

<p>If you are a student and are interested in working with me, please do not hesitate to reach out to me. <b>Specify in your email why you think we would be a good fit in terms of research interest (see my research and publication pages).</b></p>

