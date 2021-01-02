---
layout: page
title: Collaborator
permalink: /collaborator/
---

<p>I am grateful for the following people with whom I collaborated and have collaborated on various projects.  I always seek new collaboration, so I will be glad to hear from you.</p>

{% assign authors = site.data.authors %}
{% assign authors_by_sorted_last = authors | sort: 'last' %}
<ul>
{% for author in authors_by_sorted_last %}
      <li><a href="{{ author.website }}">{{ author.first }} {{ author.last }}</a> ({{ author.affiliation }})</li>
{% endfor %}
</ul>
