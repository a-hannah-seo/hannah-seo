---
layout: page
heading: All Clips
permalink: /all-clips
canonical_url: https://hannahseo.com/journalism
---

<div>
  {% assign sorted_clips = site.data.clips | sort: "date" | reverse %}
  {% assign year_groups = sorted_clips | group_by_exp: "item", "item.date | slice: 0, 4" | sort: "name" | reverse %}
  {% for group in year_groups %}
    <div class="row pad-top">
      <div class="column left-rail">
        <h3>
          {{ group.name }}
        </h3>
      </div>
      <div class="column">
        {% for clip in group.items %}
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
