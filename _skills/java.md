---
layout: default
title: Java
icon: java.png
description: "Java ha sido el lenguaje de programación base durante mi formación en DAM."
projects: [gestor-empleados]
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
