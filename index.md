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
      <!--{{ skill.title }}-->
    </a>
  {% endfor %}
</div>

## Proyectos Destacados

<div class="projects-highlight">
{% for project in site.projects limit:3 %}
  <div class="project-card">
    <p>{{ project.excerpt }}</p>
    <img src="/assets/images/{{ project.image }}" alt="{{ project.title }}">
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <!--<p>{{ project.excerpt }}</p>-->
  </div>
{% endfor %}
</div>
