---
layout: default
---

# ¡Hola 👋, Soy {{ site.title }}!

{{ site.description }}

## Sobre mí

Soy una apasionada desarrolladora con conocimiento en múltiples tecnologías. 
[Conoce más sobre mí](/about).

## Mis Habilidades

<div class="skills-grid">
  {% for skill in site.skills %}
    <a href="{{ skill.url }}" class="skill-item">
      <img src="/assets/icons/{{ skill.icon }}" alt="{{ skill.title }}">
      {{ skill.title }}
    </a>
  {% endfor %}
</div>

## Proyectos Destacados

<div class="projects-highlight">
{% for project in site.projects limit:3 %}
  <div class="project-card">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <img src="/assets/images/{{ project.image }}" alt="{{ project.title }}">
    <p>{{ project.excerpt }}</p>
  </div>
{% endfor %}
</div>
