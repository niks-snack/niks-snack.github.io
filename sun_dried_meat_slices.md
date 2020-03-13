---
layout: products
title: Продукція - М'ясні слайси в'ялені
lang: "ua"

categorie: "dried_meat_slices"
permalink: /products/dried_meat_slices/
---

{% assign sorted-posts = site.products | where: "categorie", page.categorie %}
{% for tov in sorted-posts %}
<div class="col-md-4 text-center">
<div class="menu-wrap">
    <a href="{{ tov.url }}" class="menu-img
    img mb-4" style="background-image: url(/assets/images/products/{{ tov.categorie }}/sm_{{ tov.title }}.jpg);"></a>
    <div class="text">
    <h3><a href="{{ tov.url }}">{{ tov.title_ua }}</a></h3>
    <p>{{ tov.title_text_ua | truncate: 100 }}</p>
    <p><a href="{{ tov.url }}" class="btn btn-white btn-outline-white">ПЕРЕЙТИ</a></p>
    </div>
</div>
</div>
{% endfor %}