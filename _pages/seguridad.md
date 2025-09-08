---
title: "🔐 Seguridad"
layout: single
permalink: /seguridad/
header:
  image: "/assets/images/seguridad-header.jpg"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Protección digital y buenas prácticas"
classes: wide
author_profile: true
---

## 🔐 Seguridad Digital

Explora los artículos más recientes sobre ciberseguridad, arquitectura Zero Trust y amenazas emergentes en la nube.

<div class="section-grid dark-theme">
  <div class="grid-container">
    {% assign seguridad_posts = site.categories.Seguridad %}
    {% if seguridad_posts %}
      {% assign seguridad_posts = seguridad_posts | sort: 'date' | reverse %}
      {% for post in seguridad_posts %}
        <a href="{{ post.url | relative_url }}" class="grid-item">
          <img src="{{ post.image | default: '/assets/images/seguridad-placeholder.jpg' }}" alt="{{ post.title }}">
          <div class="grid-overlay">
            <h3>{{ post.title }}</h3>
            <p>{{ post.description | default: post.excerpt }}</p>
          </div>
        </a>
      {% endfor %}
    {% else %}
      <p>No hay publicaciones disponibles en la categoría Seguridad.</p>
    {% endif %}
  </div>
</div>
