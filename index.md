---
layout: default
title: "Mi Portfolio"
---

# ¡Hola 👋, soy Tatiana Garijo Amorós!
Soy un desarrollador apasionado por la tecnología. Aquí puedes ver mis habilidades y proyectos.

## **Mis habilidades**
[🔵 Java](#java) | [🟢 SQL](#sql) | [🟡 Power BI](#pbi) | [🟡 Análisis de Datos](#ad)

## Mis habilidades
{% for skill in site.skills %}
- ![{{ skill.title }} Icon](/assets/{{ skill.icon }}.png) [{{ skill.title }}]({{ skill.url }})
{% endfor %}

## **Mis proyectos**
{% for project in site.projects %}
- [{{ project.title }}]({{ project.url }})
{% endfor %}
