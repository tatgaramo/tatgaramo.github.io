---
layout: default
title: "JAVA"
icon: "java.png"
url: "/skills/java"
description: "Java ha sido el lenguaje de programación base durante mi formación en DAM."
projects:
  - name: "Calculadora"
    image: "java.png"
    url: "[https://ejemplo.com/calc](https://tatgaramo.github.io/)"
  
---

# JAVA
Mi conocimiento en Java me ha permitido trabajar en proyectos como:

{% for project in page.projects %}
<div class="project">
  <h3>{{ project.name }}</h3>
  <img src="/assets/images/{{ project.image }}" alt="{{ project.name }}">
  <a href="{{ project.url }}">Ver proyecto</a>
</div>
{% endfor %}
