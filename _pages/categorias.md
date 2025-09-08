---
title: "Categorías"
layout: categories
permalink: /categorias/
header:
  image: "/assets/images/header.jpg"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Explora los temas del blog"
---

Selecciona una categoría para ver artículos relacionados:

- 🍎 Apple
- 🪟 Microsoft
- 🔐 Seguridad
- 🌐 VPN

Este espacio se actualizará automáticamente conforme publiques artículos con etiquetas.
---

## 🗂️ Reseñas destacadas

{% assign all_categories = "Apple,Microsoft,Seguridad,VPN" | split: "," %}
{% for category in all_categories %}
  {% assign posts = site.categories[category] | sort: 'date' | reverse %}
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
