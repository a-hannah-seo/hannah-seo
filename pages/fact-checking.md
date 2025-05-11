---
permalink: /fact-checking
layout: page
heading: Fact Checking
contact_link: /contact
---

<div class="row pad-top">
  <div class="column left-rail">

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
    
    <p> Cupcake ipsum dolor sit amet. Pie pie sugar plum topping brownie oat cake. Caramels apple pie muffin cake chocolate bar cake. </p>
    
    <p> Jelly-o chocolate bear claw danish jelly beans chupa chups tootsie roll gingerbread macaroon. Tootsie roll oat cake jujubes tart muffin powder brownie tart jelly-o. Pastry sugar plum caramels shortbread donut candy powder shortbread tiramisu. Shortbread powder gummies dragée icing dessert brownie marshmallow toffee. </p>

    <p> Gingerbread lemon drops wafer ice cream croissant soufflé jelly-o pastry. Cake cheesecake carrot cake shortbread jelly beans powder dessert sweet. Wafer icing chocolate tootsie roll chupa chups ice cream bonbon. Jelly-o liquorice jelly-o danish topping bear claw. </p>

  </div>
</div>
