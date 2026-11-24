---
layout: page
title: projects
permalink: /projects/
description: Research in progress.
nav: true
nav_order: 3
---

{% assign sorted_projects = site.projects | sort: "importance" %}

<ul class="jt-projects">
{% for project in sorted_projects %}
  <li class="jt-project">
    <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
    {% if project.description %}<p class="jt-project-meta">{{ project.description }}</p>{% endif %}
    {% if project.summary %}<p class="jt-project-summary">{{ project.summary }}</p>{% endif %}
    {% if project.pdf %}<p class="jt-project-links"><a href="{{ project.pdf | relative_url }}">PDF</a></p>{% endif %}
  </li>
{% endfor %}
</ul>
