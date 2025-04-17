---
layout: default
---

# ¡Hola 👋, Soy {{ site.title }}!

{{ site.description }}

## Sobre mí

Soy una apasionada desarrolladora con conocimiento en múltiples tecnologías. 
[Conoce más sobre mí](/about).

## Mis Habilidades

<div class="skills-container">
{% for skill in site.skills %}
  <div class="skill-card">
    <a href="{{ skill.url }}">
      <img src="/assets/icons/{{ skill.icon }}" alt="{{ skill.title }}" class="skill-icon">
      <h3>{{ skill.title }}</h3>
    </a>
    <p>{{ skill.description }}</p>
  </div>
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
