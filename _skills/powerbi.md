---
layout: default
title: Power BI
icon: pbi.svg
description: " He estado aprendido Power BI para la visualización y análisis de datos."
projects:
  - pbi-1.md
---

# {{ page.title }}

{{ page.description }}

## Mis Proyectos con {{ page.title }}

{% for project_name in page.projects %}
  {% assign project = site.projects | where: "slug", project_name | first %}
  {% if project %}
    <div class="project-item">
      <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
      <img src="/assets/images/{{ project.image }}" alt="{{ project.title }}">
      <p>{{ project.description }}</p>
      <a href="{{ project.demo_url }}" class="btn">Ver Demo</a>
      <a href="{{ project.repo_url }}" class="btn">Código Fuente</a>
    </div>
  {% endif %}
{% endfor %}

[Volver al inicio](/)
