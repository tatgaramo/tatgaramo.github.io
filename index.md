---
layout: default
---

# ¡Hola 👋, Soy {{ site.title }}!

<h2>Desarrolladora de software y aplicaciones multiplataforma 💻</h2>

##👩 Sobre mí

Soy una apasionada desarrolladora con conocimiento en múltiples tecnologías. 
[Conoce más sobre mí](/about).
<div class="social-links">
      <a href="https://github.com/{{ site.social.github }}" target="_blank" rel="noopener">
        <img src="/assets/icons/github.svg" alt="GitHub" width="24" height="24">
      </a>
      <a href="https://linkedin.com/in/{{ site.social.linkedin }}" target="_blank" rel="noopener">
        <img src="/assets/icons/linkedin.png" alt="LinkedIn" width="24" height="24">
      </a>
      <a href="mailto:{{ site.social.email }}">
        <img src="/assets/icons/email.svg" alt="Email" width="24" height="24">
      </a>
    </div>

## 📋 Mis Habilidades

<div class="skills-grid">
  {% for skill in site.skills %}
    <a href="{{ skill.url }}" class="skill-item">
      <img src="/assets/icons/{{ skill.icon }}" alt="{{ skill.title }}" class="skill-icon">
      <span class="skill-title">{{ skill.title }}</span>
    </a>
  {% endfor %}
</div>

## ✨Proyectos Destacados 

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
