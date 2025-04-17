---
layout: default
title: Proyecto curso IBM - Datahack
slug: pbi-1
image: gestor-empleados.png
description: Informe para el análisis y visualizacion de datos, proyecto del curso realizado IBM-Datahack
technologies: [Power BI]
demo_url: https://app.powerbi.com/view?r=eyJrIjoiMjk3ODMwOWEtZTJmNi00MjAyLWE3ZWMtOTUwYzRmY2RhMDY2IiwidCI6IjQzYTllNTAwLWY5YmMtNGZmZi04OGFhLTBhMjg4ZTdhNzhlZiJ9
<!--repo_url: https://github.com/tuusuario/gestor-empleados-->
---

# {{ page.title }}

![Captura del proyecto](/assets/images/{{ page.image }})

## Descripción

Informe para el análisis y visualizacion de datos de Google ads:
- Visualización de informe interacativo
- Análisis da datos
- .....

## Tecnologías utilizadas

{% for tech in page.technologies %}
- {{ tech }}
{% endfor %}

## Enlaces

[Ver]({{ page.demo_url }}) | 
[Repositorio en GitHub]({{ page.repo_url }})

[Volver a Java](/skills/java) | 
[Volver al inicio](/)
