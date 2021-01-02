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
      <li>{{ authors[key].first }} {{ authors[key].last }} ({{ authors[key].affiliation }})</li>
{% endfor %}
</ul>
