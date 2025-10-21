---
title: "🧱 Infraestructura"
layout: single
permalink: /infraestructura/
header:
  image: "/assets/images/infraestructura-header-bnw.png"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Servidores, DNS, cloud y automatización técnica"
classes: wide
author_profile: true
---

## 🧱 Ecosistema de Infraestructura

Explora el mundo de servidores, DNS, cloud, automatización y arquitectura digital.  
Aquí encontrarás guías, análisis y configuraciones para entornos técnicos y empresariales.

<div class="section-grid dark-theme">
  <div class="grid-container">
    {% assign infraestructura_posts = site.categories.Infraestructura %}
    {% if infraestructura_posts %}
      {% assign infraestructura_posts = infraestructura_posts | sort: 'date' | reverse %}
      {% for post in infraestructura_posts %}
        <a href="{{ post.url | relative_url }}" class="grid-item">
          <img src="{{ post.image | default: '/assets/images/infraestructura-placeholder.jpg' }}" alt="{{ post.title }}">
          <div class="grid-overlay">
            <h3>{{ post.title }}</h3>
            <p>{{ post.description | default: post.excerpt }}</p>
          </div>
        </a>
      {% endfor %}
    {% else %}
      <p>No hay publicaciones disponibles en la categoría Infraestructura.</p>
    {% endif %}
  </div>
</div>