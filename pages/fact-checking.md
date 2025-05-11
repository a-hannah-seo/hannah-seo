---
permalink: /fact-checking
layout: page
heading: Fact Checking
contact_link: /contact
---

<div class="row pad-top">
  <div class="column left-rail">
  <div>
    <h3><a href="{{page.contact_link}}">Contact me</a></h3>
  </div>

  {% for t in site.data.faxx %}
    <div class="testimonial">
      <h4>
        <a href="{{t.link}}" target="_blank">
        {{t.name}}. <i>{{t.title}}</i>. {{t.publisher}}, {{t.year}}.
        </a>
      </h4>
      <p>{{t.body}}</p>
    </div>
  {% endfor %}
  </div>
  <div class="column">

    <h2>tktktk</h2>
    <p> tktktk </p>

  </div>
</div>
