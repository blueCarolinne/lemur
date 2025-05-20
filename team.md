---
title: Equipo
layout: teams
description: Nuestro equipo
permalink: "/team/"
intro_image_absolute: true
intro_image_hide_on_mobile: false
---

# Profesores

{% assign profesores = site.team | where: "category", "profesor" %}
<div class="_team-grid">
  {% for person in profesores %}
    {% include team-member.html member=person %}
  {% endfor %}
</div>

# Estudiantes

{% assign estudiantes = site.team | where: "category", "estudiante" %}
<div class="team-grid">
  {% for person in estudiantes %}
    {% include team-member.html member=person %}
  {% endfor %}
</div>
