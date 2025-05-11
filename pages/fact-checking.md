---
permalink: /fact-check
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
        {{t.title}}
      </h4>
      <p>{{t.body}}</p>  
      <p>— {{t.name}}, {{t.date}}</p>
    </div>
  {% endfor %}
  </div>
  <div class="column">

    <h2>tktktk</h2>
    <p> tktktk </p>

  </div>
</div>
