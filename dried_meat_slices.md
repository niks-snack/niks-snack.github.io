---
layout: products
lang: "ua"

slider_bottom_1: "Дома та в дорозі ВКЛючайся з нами!"
slider_bottom_2: "ВКЛючай смак!"
slider_bottom_3: "ВКЛючай емоції!"

categorie: "sun_dried_meat_slices"
permalink: /products/sun_dried_meat_slices/
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