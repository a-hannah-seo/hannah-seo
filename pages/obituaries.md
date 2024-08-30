---
permalink: /obituaries
layout: page
heading: Obituaries
contact_link: /contact
---

<div class="row pad-top">
  <div class="column left-rail">
  <div>
    <h3><a href="{{page.contact_link}}">Contact me</a></h3>
  </div>

  {% for t in site.data.obit_t %}
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

    <h1>Est debitis voluptas et repellat pariatur.</h1>
    <p>Lorem ipsum dolor sit amet. Qui omnis similique <em>Aut similique et tempore velit ut galisum quasi</em>? Eum perspiciatis consequaturCum voluptate aut nulla provident et cumque minus. Ut recusandae quia est maxime nesciunt <strong>Ut repudiandae et ullam similique sed ducimus beatae est tenetur maxime</strong> non internos fugit. </p>

    <h2>Non reprehenderit voluptas et vero numquam et temporibus quaerat. </h2>
    <p>Sit placeat unde <em>Eum quae et quasi ullam sed praesentium quasi</em> qui dolores pariatur ut inventore reiciendis. Vel perspiciatis voluptateQuo deserunt ut blanditiis iusto qui quaerat omnis. In quisquam minima <strong>Nam ducimus et nihil dolores et magni velit</strong> non quas dicta? </p>

    <h3>Ea impedit recusandae non facere eius. </h3>
    <p>Ex repellendus minusQuo optio eos laboriosam suscipit in molestias mollitia et labore labore. Qui consequatur accusamus <em>Vel dolor rem aperiam ratione At earum molestiae</em> sed nihil blanditiis. Sed consequuntur omnis <strong>Et accusamus 33 voluptatem facere vel adipisci maiores et ipsum tempora</strong>? Ex voluptatibus nisiEt Quis qui fuga laborum sed sint quidem ut dolor velit nam adipisci impedit. </p>
  </div>
</div>
