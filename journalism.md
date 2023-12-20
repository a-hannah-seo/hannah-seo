---
layout: page
title: Journalism
permalink: /journalism/
priority: 1
---


<div class="article-box">
  {% for article in site.data.articles %}
    <div class="article">
      <img class="article-image" src="{{ article.image }}" alt="{{ article.alt-text }}"/>
      <div class="article-text">
        <p><span class="article-highlight article-title"> "{{ article.title }}" </span></p>
        <p><span class="article-highlight"> {{ article.blurb }} </span></p>
        <p><span class="article-highlight"><i><a href="{{ article.link }}"> {{ article.publication }} </a></i></span></p>
      </div>
    </div>
  {% endfor %}
</div>

