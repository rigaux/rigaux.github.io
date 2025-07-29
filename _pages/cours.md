---
layout: page
title: Cours
permalink: /cours/
description: Liste des support de cours
nav: true
nav_order: 3
horizontal: false
---

<!-- pages/cours.md -->
<div class="projects">

<!-- Affichage de la liste des cours -->

<p>Chacun de mes cours est accessible sous la forme d'un site web organisé
en chapitre et sections, comprenant un texte détaillé, une vidéo 
résumant les points-clé, des exercices et des quiz.</p>

{% assign les_cours = site.cours | sort: "importance" %}

  <!-- Une petite carte pour chaque cours -->

  <div class="row row-cols-1 row-cols-md-3">
    {% for cours in les_cours %}
      {% include cours.liquid %}
    {% endfor %}
  </div>
</div>
