---
layout: page
title: Poetry
permalink: /poetry
priority: 2
description: "Poetry by Hannah Seo, published in Palette Poetry, Witness Magazine, Pedestal Magazine, and other journals."
---

<div class="poem-box pad-top">
  {% for poem in site.data.poems %}
    <div class="poem">
      <img class="poem-image" src="{{ poem.image }}" alt="{{ poem.alt-text }}"/>
      <div class="poem-text">
        <p><span class="poem-highlight poem-title"> {{ poem.title }} </span></p>
        <p><span class="poem-highlight"> {{ poem.blurb }} </span></p>
        <p><span class="poem-highlight"><i><a href="{{ poem.link }}"> {{ poem.publication }} </a></i></span></p>
      </div>
    </div>
  {% endfor %}
</div>

