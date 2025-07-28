---
layout: page
title: Cours
permalink: /cours/
description: Cours
nav: true
nav_order: 5
horizontal: false
---

<!-- pages/cours.md -->
<div class="projects">

<!-- Affichage de la liste des cours -->

{% assign les_cours = site.cours | sort: "importance" %}

  <!-- Generate cards for each project -->

  <div class="row row-cols-1 row-cols-md-3">
    {% for cours in les_cours %}
      {% include cours.liquid %}
    {% endfor %}
  </div>
</div>
