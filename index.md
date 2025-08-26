---
layout: splash
title: "Blog de Tecnología y Seguridad Digital"
header:
  image: "/assets/images/header.jpg"
  overlay_color: "#000"
  overlay_filter: "0.3"
  caption: "Tecnología que inspira confianza"
  actions:
    - label: "Ver artículos"
      url: "/categorias/"
feature_row:
  - image_path: /assets/images/apple.png
    title: "Apple"
    excerpt: "macOS, iOS, hardware y seguridad"
    url: "/apple/"
    btn_label: "Ver artículos"
    btn_class: "btn--primary"
  - image_path: /assets/images/windows.png
    title: "Microsoft"
    excerpt: "Herramientas, productividad y seguridad"
    url: "/microsoft/"
    btn_label: "Ver artículos"
    btn_class: "btn--primary"
  - image_path: /assets/images/security.png
    title: "Seguridad"
    excerpt: "Protección de datos y buenas prácticas"
    url: "/seguridad/"
    btn_label: "Ver artículos"
    btn_class: "btn--primary"
  - image_path: /assets/images/vpn.png
    title: "VPN"
    excerpt: "Privacidad y navegación segura"
    url: "/vpn/"
    btn_label: "Ver artículos"
    btn_class: "btn--primary"
---

Bienvenido a mi espacio técnico. Aquí encontrarás análisis, guías y recursos sobre:

- 🍎 Apple: ecosistema, configuraciones y novedades  
- 🪟 Microsoft: productividad, seguridad y herramientas  
- 🔐 Seguridad digital: buenas prácticas y protección de datos  
- 🌐 VPN: privacidad, navegación segura y acceso remoto  

<body>
  <!-- Tu contenido principal -->
  <div id="visitas">Visitantes: cargando...</div>

  <!-- Script de CountAPI -->
  <script>
    fetch('https://api.countapi.xyz/hit/pcsupportslp.com/visitas')
      .then(res => res.json())
      .then(data => {
        document.getElementById('visitas').innerText = 'Visitantes: ' + data.value;
      });
  </script>
</body>
Este blog está diseñado para ofrecer una experiencia clara, profesional y en modo oscuro. ¡Explora y aprende!



{% include feature_row %}


