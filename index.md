---
layout: default
---

# ¡Hola 👋, Soy {{ site.title }}!

<h2>Estudiante DAM | Desarrollo de software y aplicaciones multiplataforma.</h2>

## Sobre mí

Soy una apasionada desarrolladora con conocimiento en múltiples tecnologías. 
[Conoce más sobre mí](/about).

## Mis Habilidades

<div class="skills-grid">
  {% for skill in site.skills %}
    <a href="{{ skill.url }}" class="skill-item">
      <img src="/assets/icons/{{ skill.png }}" alt="{{ skill.title }}">
      {{ skill.title }}
    </a>
  {% endfor %}
</div>

## Proyectos Destacados

<div class="projects-grid">
  {% for project in site.projects limit:3 %}
    <div class="project-tile">
      <a href="{{ project.url }}">
        <img src="/assets/images/{{ project.image }}" alt="{{ project.title }}">
        <div class="project-overlay">{{ project.title }}</div>
      </a>
    </div>
  {% endfor %}
</div>
</div>
