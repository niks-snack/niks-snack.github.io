---
pub: "yes"
layout: products
lang: "ua"
meta_description: "Купити в Україні Сушені гриби"
categorie: "dried_mushrooms"
permalink: /products/dried_mushrooms/
---

{% assign sorted-posts = site.products | where: "categorie", page.categorie %}
{% assign sorted-posts = sorted-posts | where: "lang", "ua" %}
{% for tov in sorted-posts %}
<div class="col-md-4 text-center">
<div class="menu-wrap">
    <a href="{{ tov.url }}" class="menu-img
    img mb-4" style="background-image: url(/assets/images/products/{{ tov.categorie }}/sm_{{ tov.title }}.jpg);"></a>
    <div class="text">
    <h3><a href="{{ tov.url }}">{{ tov.title_small }}</a></h3>
    <p>{{ tov.title_text | truncate: 100 }}</p>
    <p><a href="{{ tov.url }}" class="btn btn-white btn-outline-white">ПЕРЕЙТИ</a></p>
    </div>
</div>
</div>
{% endfor %}