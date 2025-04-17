---
layout: default
title: "Mi Portfolio"
---

# ¡Hola 👋, soy Tatiana Garijo Amorós!
Soy un desarrollador apasionado por la tecnología. Aquí puedes ver mis habilidades y proyectos.

## Sobre mí
Breve descripción sobre ti y tu experiencia.

## **Mis habilidades1**
[🔵 Java](#java) | [🟢 SQL](#sql) | [🟡 Power BI](#pbi) | [🟡 Análisis de Datos](#ad)

## Mis habilidades2
{% for skill in site.skills %}
- ![{{ skill.title }} Icon](/assets/icons/{{ skill.icon }}.png) [{{ skill.title }}]({{ skill.url }})
{% endfor %}

## Habilidades3

{% for skill in site.skills %}
<div class="skill-item">
  <a href="{{ skill.url }}">
    <img src="/assets/icons/{{ skill.icon }}" alt="{{ skill.title }}" width="50">
    <h3>{{ skill.title }}</h3>
  </a>
</div>
{% endfor %}

## **Mis proyectos**
{% for project in site.projects %}
- [{{ project.title }}]({{ project.url }})
{% endfor %}
