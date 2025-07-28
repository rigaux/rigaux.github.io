---
layout: page
title: Modèle relationnel
permalink: /modrel/
description: Cours
nav: false
nav_order: 5
horizontal: false
---

<!-- pages/cours.md -->
<div class="projects">

<!-- Affichage de la liste des cours -->

{% assign les_chapitres = site.modrel  %}

  <!-- Generate cards for each project -->

  <div class="row row-cols-1 row-cols-md-3">
    {% for project in les_chapitres %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
</div>
