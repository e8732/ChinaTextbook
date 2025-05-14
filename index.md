---
layout: default
---
## PDF文件列表
{% for file in site.static_files %}
  {% if file.path contains '/pdfs/' %}
  - [{{ file.name }}]({{ file.path }})
% endif %}
{% endfor %}
