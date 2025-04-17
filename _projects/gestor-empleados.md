---
layout: default
title: Gestor de Empleados
slug: gestor-empleados
image: gestor-empleados.png
description: Sistema completo para gestión de empleados con Java, Hibernate, Swing
technologies: [Java, Swing, Hibernate, MySQL]
<!--demo_url: https://demo.com/gestor-empleados
repo_url: https://github.com/tuusuario/gestor-empleados-->
---

# {{ page.title }}

<!-- Imagen principal -->
<img src="/assets/images/{{ page.slug }}.png" alt="{{ page.title }}">
<div class="image-grid">
<!-- Imágenes adicionales -->
{% for i in (1..4) %}
  <img src="/assets/images/{{ page.slug }}-{{ i }}.png" 
       alt="{{ page.title }} captura {{ i }}"
       loading="lazy">>
{% endfor %}
  </div>
<!--![Captura del proyecto](/assets/images/{{ page.image }})-->


## Descripción

Sistema completo desarrollado con Java e Hibernate que permite:
- Gestión de empleados
- Operaciones CRUD
- Exportar e importar

## Tecnologías utilizadas

{% for tech in page.technologies %}
- {{ tech }}
{% endfor %}

## Enlaces

[Ver demo en vivo]({{ page.demo_url }}) | 
[Repositorio en GitHub]({{ page.repo_url }})

[Volver a Java](/skills/java) | 
[Volver al inicio](/)
