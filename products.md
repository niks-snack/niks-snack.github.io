---
layout: products
title: Jekyll products
---

{% for products in site.products %}

<a href="{{ products.url | prepend: site.baseurl }}">
  <h2>{{ products.title }}</h2>
</a>

<p class="post-excerpt">{{ products.description | truncate: 160 }}</p>

{% endfor %}