---
layout: default
---

<h1 class="page-title">Авторские украшения ручной работы</h1>
<div class="product-grid">

  {% for product in site.products %}

    <a class="product-card" href="{{ product.url | relative_url }}">
      
      <div class="product-image">
        <img src="{{ product.image | relative_url }}" alt="{{ product.title }}">
      </div>

      <div class="product-info">
        <p class="product-price">{{ product.price_display }}</p>
      </div>

    </a>

  {% endfor %}

</div>