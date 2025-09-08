---
title: "Categorías"
layout: single
permalink: /categorias/
header:
  image: "/assets/images/header.jpg"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Explora los temas del blog"
---

Selecciona una categoría para ver artículos relacionados:

- 🍎 [Apple](/apple/)
- 🪟 [Microsoft](/microsoft/)
- 🔐 [Seguridad](/seguridad/)
- 🌐 [VPN](/vpn/)

Este espacio se actualizará automáticamente conforme publiques artículos con etiquetas.

---

## 🗂️ Reseñas destacadas

### 🍎 Apple

{% assign apple_posts = site.categories.Apple | sort: 'date' | reverse %}
{% for post in apple_posts %}
  {% include archive-single.html %}
{% endfor %}

### 🪟 Microsoft

{% assign microsoft_posts = site.categories.Microsoft | sort: 'date' | reverse %}
{% for post in microsoft_posts %}
  {% include archive-single.html %}
{% endfor %}

### 🔐 Seguridad

{% assign seguridad_posts = site.categories.Seguridad | sort: 'date' | reverse %}
{% for post in seguridad_posts %}
  {% include archive-single.html %}
{% endfor %}

### 🌐 VPN

{% assign vpn_posts = site.categories.VPN | sort: 'date' | reverse %}
{% for post in vpn_posts %}
  {% include archive-single.html %}
{% endfor %}
