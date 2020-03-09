---
layout: products
title: Jekyll products
---

{% for products in site.products %}

<a href="{{ products.url }}">{{ products.title }}</a>

<p class="post-excerpt">{{ products.description | truncate: 160 }}</p>

{% endfor %}