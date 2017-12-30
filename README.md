---
layout: default
permalink: index.html
redirect_from:
  - /libraries.html
  - /projects.html
---

<!-- Comment to prevent automatic title assignment -->
# Welcome

Welcome to the Macchina Community Showcase!  Here you will find all kinds of resources related to Macchina hardware.

## Libraries

<!-- to add a library add it in _data/arduino-libraries.yml -->

{% assign libraries = site.data.arduino-libraries | sort: 'name' %}
{%- for library in libraries -%}
- [{{ library.name }}]({{ library.url }}) - {{ library.description }}
{% endfor %}


## Projects

<!-- to add a project add it in _data/projects.yml -->

{% assign projects = site.data.projects | sort: 'name' %}
{%- for project in projects -%}
- [{{ project.name }}]({{ project.url }}) - {{ project.description }}
{% endfor %}

## Contributing

This website exists to help connect users to projects, ideas, and other resources.  If you know something that should be listed here, please let us know on GitHub by opening an [Issue](https://github.com/macchina/showcase/issues) or submitting a [Pull Request](https://github.com/macchina/showcase/pulls).