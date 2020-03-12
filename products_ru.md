---
layout: products
title: Продукция
---

{% for products in site.products %}
<div class="col-md-4 text-center">
    <div class="menu-wrap">
      <a href="#" class="menu-img
       img mb-4" style="background-image: url(assets/images/sm_{{ products.title }}.jpg);"></a>
      <div class="text">
        <h3><a href="{{ products.url }}">{{ products.title_ru }}</a></h3>
        <p>{{ products.title_text_ua | truncate: 100 }}</p>
        <p><a href="{{ products.url }}" class="btn btn-white btn-outline-white">Открыть</a></p>
      </div>
    </div>
  </div>
{% endfor %}