---
title: "🪟 Microsoft"
layout: single
permalink: /microsoft/
header:
  image: "/assets/images/microsoft-header.jpg"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Tecnología empresarial y productividad"
classes: wide
author_profile: true
---

## 🪟 Ecosistema Microsoft

Explora el mundo de Windows, Office, Azure y herramientas de productividad.  
Aquí encontrarás guías, reseñas y configuraciones para entornos personales y profesionales.

<div class="section-grid dark-theme">
  <div class="grid-container">
    {% assign microsoft_posts = site.categories.Microsoft %}
    {% if microsoft_posts %}
      {% assign microsoft_posts = microsoft_posts | sort: 'date' | reverse %}
      {% for post in microsoft_posts %}
        <a href="{{ post.url | relative_url }}" class="grid-item">
          <img src="{{ post.image | default: '/assets/images/microsoft-placeholder.jpg' }}" alt="{{ post.title }}">
          <div class="grid-overlay">
            <h3>{{ post.title }}</h3>
            <p>{{ post.description | default: post.excerpt }}</p>
          </div>
        </a>
      {% endfor %}
    {% else %}
      <p>No hay publicaciones disponibles en la categoría Microsoft.</p>
    {% endif %}
  </div>
</div>
