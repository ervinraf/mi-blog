{% assign apple_posts = site.categories.Apple %}
{% if apple_posts %}
  {% assign apple_posts = apple_posts | sort: 'date' | reverse %}
  {% for post in apple_posts %}
    <a href="{{ post.url | relative_url }}" class="grid-item">
      <img src="{{ post.image | default: '/assets/images/apple-placeholder.jpg' }}" alt="{{ post.title }}">
      <div class="grid-overlay">
        <h3>{{ post.title }}</h3>
        <p>{{ post.description | default: post.excerpt }}</p>
      </div>
    </a>
  {% endfor %}
{% else %}
  <p>No hay publicaciones disponibles en la categoría Apple.</p>
{% endif %}
