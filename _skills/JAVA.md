---
title: "JAVA"
icon: "java.png"
url: "/skills/java"
description: "Java ha sido el lenguaje de programación base durante mi formación en DAM."
layout: skill
projects:
  - Gestor-empleados
  - Gestor-Academia
---

# JAVA
Mi conocimiento en Java me ha permitido trabajar en proyectos como:
{% for project in site.projects %}
{% if project.title in page.projects %}
- [{{ project.title }}]({{ project.url }}) - {{ project.description }}
{% endif %}
{% endfor %}
