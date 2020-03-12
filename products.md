---
layout: products
title: Продукція
lang: "ua"

slider_bottom_1: "Дома та в дорозі ВКЛючайся з нами!"
slider_bottom_2: "ВКЛючай смак!"
slider_bottom_3: "ВКЛючай емоції!"
---

{% for products in site.products %}
<div class="col-md-4 text-center">
    <div class="menu-wrap">
      <a href="{{ products.url }}" class="menu-img
       img mb-4" style="background-image: url(assets/images/products/{{ products.categorie }}/sm_{{ products.title }}.jpg);"></a>
      <div class="text">
        <h3><a href="{{ products.url }}">{{ products.title_ua }}</a></h3>
        <p>{{ products.title_text_ua | truncate: 100 }}</p>
        <p><a href="{{ products.url }}" class="btn btn-white btn-outline-white">Відкрити</a></p>
      </div>
    </div>
  </div>
{% endfor %}