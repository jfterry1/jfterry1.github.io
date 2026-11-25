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
  <li class="jt-project{% if project.figure %} has-figure{% endif %}">
    <div class="jt-project-text">
      <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
      {% if project.description %}<p class="jt-project-meta">{{ project.description }}</p>{% endif %}
      {% if project.summary %}<p class="jt-project-summary">{{ project.summary }}</p>{% endif %}
      {% if project.pdf %}<p class="jt-project-links"><a href="{{ project.pdf | relative_url }}">PDF</a></p>{% endif %}
    </div>
    {% if project.figure %}
    <a class="jt-project-thumb" href="{{ project.url | relative_url }}" tabindex="-1" aria-hidden="true">
      <img src="{{ project.figure | relative_url }}" alt="" loading="lazy">
    </a>
    {% endif %}
  </li>
{% endfor %}
</ul>
