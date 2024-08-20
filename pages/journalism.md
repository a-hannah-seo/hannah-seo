---
layout: page
title: Journalism
heading: Selected Works
permalink: /journalism
clips-link: /all-clips
priority: 1
---

<div class="article-box pad-top">
  {% for article in site.data.articles %}
    <div class="article">
      <img class="article-image" src="{{ article.image }}" alt="{{ article.alt-text }}"/>
      <div class="article-text">
        <p><span class="article-highlight article-title"> {{ article.title }} </span></p>
        <p><span class="article-highlight"> {{ article.blurb }} </span></p>
        <p><span class="article-highlight"><i><a href="{{ article.link }}"> {{ article.publication }} </a></i></span></p>
      </div>
    </div>
  {% endfor %}
</div>

<br/>
<div class="push-right">
  <p>
    <a href="{{ page.clips-link }}">See all clips here.</a> 
  </p>
</div>
