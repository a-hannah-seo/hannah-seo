---
layout: page
title: Audio
permalink: /audio/
priority: 3
---

<div class="row">
  <div class="column left-rail">
    <h3>
      🎤🎙📻
    </h3>
  </div>
  <div class="column">
    <ul>
      {% for clip in site.data.clips %}
        <li class="boom">
          {{ clip.role }} on <u>{{ clip.title }}</u>, for <a href="{{ clip.link }}">{{ clip.publication }}</a>
        </li>
      {% endfor %}
    </ul>

</div>

