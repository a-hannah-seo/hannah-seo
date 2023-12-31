---
layout: page
title: Audio
permalink: /audio
priority: 3
supported_roles: [appearances, credits]
---
<div>
{% for role in page.supported_roles %}
  {% assign clips = site.data.audio | where: "role", role %}
  <div class="row pad-top">
    <div class="column left-rail">
      <h3>
        {{ role }}
      </h3>
    </div>
    <div class="column">
      {% for clip in clips %}
      <div>
        <a href="{{ clip.link }}"><u>{{ clip.title }}</u></a>
        <br/>
        <i>{{ clip.credit }} for {{ clip.publication }}, {{ clip.date }}</i>
        <ul>
          <li class="boom">
            {{ clip.blurb }}
          </li>
        </ul>
      </div>
      {% endfor %}
    </div>
  </div>
{% endfor %}
</div>