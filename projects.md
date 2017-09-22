---
title: Projects
---

<!-- to add a project add it in _data/projects.yml -->

{% assign projects = site.data.projects | sort: 'name' %}
{%- for project in projects -%}
- [{{ project.name }}]({{ project.url }}) - {{ project.description }}
{% endfor %}