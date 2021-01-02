---
layout: page
title: Collaborator
permalink: /collaborator/
---

<p>I am grateful for the following people with whom I collaborated and have collaborated on various projects.</p>

{% assign authors = site.data.authors %}
<ul>
{% for author in authors %}
      <li><a href="{{ authors[author].website }}">{{ authors[author].first }} {{ authors[author].last }}</a> ({{ authors[author].affiliation }})</li>
{% endfor %}
</ul>
