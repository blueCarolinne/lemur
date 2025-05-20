---
title: Equipo
layout: teams
description: Nuestro equipo
permalink: "/team/"
intro_image_absolute: true
intro_image_hide_on_mobile: false
---



# Profesores

{% assign profesor = site.team | where: "category", "profesor" %}
<div class="team-grid">
  {% for person in profesor %}
    {% include team-member.html member=person %}
  {% endfor %}
</div>

# Estudiantes

{% assign estudiante = site.team | where: "category", "estudiante" %}
<div class="team-grid">
  {% for person in estudiante %}
    {% include team-member.html member=person %}
  {% endfor %}
</div>
