---
layout: page
title: Publication
permalink: /publication/
---

This page contains a list of my publications in a chronological order.
If you have questions regarding any of these publications, please feel free to contact me.

<ul>
{% for pub in site.publications %}
<li>
  {{ pub.title }}
</li>
{% endfor %}
<ul>
