---
layout: default
title: Essays
---

<h1>Essays</h1>

<ul class="essay-list">
{% assign sorted_essays = site.essays | sort: "date" | reverse %}
{% for essay in sorted_essays %}
  <li>
    <time datetime="{{ essay.date | date_to_xmlschema }}">{{ essay.date | date: "%b %-d, %Y" }}</time>
    <a href="{{ essay.url | relative_url }}">{{ essay.title }}</a>
  </li>
{% endfor %}
</ul>
