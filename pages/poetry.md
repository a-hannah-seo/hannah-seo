---
layout: page
title: Poetry
permalink: /poetry
priority: 2
---

<div class="poem-box">
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

