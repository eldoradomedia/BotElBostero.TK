---
layout: default
title: Partidos del CA Peñarol / Temporada 2024
author: elbosterobot.tk
---

<div class="espacio kustom_culture">
  <h2>{{ page.title }}</h2>
</div>
<!--<div class="kustom_culture">
  {% for post in site.posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a><br>
  </li>
  {% endfor %}
</div>-->

<div class="cover">
  <button class="left" onclick="leftScroll()">
    <i class="fas fa-angle-double-left"></i>
  </button>
  <div class="scroll-images">
    {% for post in site.posts %}
    <div class="child">
      <div class="card m-2">
        <div class="card-header text-center kustom_culture">{{ post.category }} · JORNADA {{ post.jornada }}</div>
        <img src="{{ site.url }}{{ post.image }}" width="100%">
        <div class="card-body">
          <h2 class="card-title kustom_culture">{{ post.local }} X<br>
          {{ post.visitante }}</h2>
          <span class="card-text dyuthi_regular">Relato: {{ post.relato }}</span><br>
          <a href="{{ post.url }}" class="btn btn-dark kustom_culture">Ver Online </a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
  <button class="right" onclick="rightScroll()">
    <i class="fas fa-angle-double-right"></i>
  </button>
</div>
