---
title: "JAVA"
icon: "java"
description: "Java ha sido el lenguaje de programación base durante mi formación en DAM."
layout: skill
projects:
  - Gestor-empleados
  - Gestor-Academia
---

# HTML
Mi conocimiento en Java me ha permitido trabajar en proyectos como:
{% for project in site.projects %}
{% if project.title in page.projects %}
- [{{ project.title }}]({{ project.url }}) - {{ project.description }}
{% endif %}
{% endfor %}
