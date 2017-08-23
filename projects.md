---
title: Projects
---

{% assign projects = site.data.projects | sort: 'name' %}
{%- for project in projects -%}
- [{{ project.name }}]({{ project.url }}) - {{ project.description }}
{% endfor %}