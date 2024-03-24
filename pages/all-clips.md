---
layout: page
heading: All Clips
permalink: /all-clips
---

<div>
  {% assign years = site.data.clips | map: "year" | uniq %}
  {% for year in years %}
    {% assign clips = site.data.clips | where: "year", year %}
    <div class="row pad-top">
      <div class="column left-rail">
        <h3>
          {{ year }}
        </h3>
      </div>
      <div class="column">
        {% for clip in clips %}
        <div>
          <a href="{{ clip.link }}"><u>{{ clip.title }}</u></a>
          <br/>
          <i>{{ clip.publication }}</i>
        </div>
        {% endfor %}
      </div>
    </div>
  {% endfor %}
</div>
