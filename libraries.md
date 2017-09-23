---
title: Libraries
edit_path: _data/arduino-libraries.yml
---

<!-- to add a library add it in _data/arduino-libraries.yml -->

{% assign libraries = site.data.arduino-libraries | sort: 'name' %}
{%- for library in libraries -%}
- [{{ library.name }}]({{ library.url }}) - {{ library.description }}
{% endfor %}