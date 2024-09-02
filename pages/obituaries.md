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

    <h2>Est debitis voluptas et repellat pariatur.</h2>
    <p>Lorem ipsum dolor sit amet. Qui omnis similique <em>Aut similique et tempore velit ut galisum quasi</em>? Eum perspiciatis consequaturCum voluptate aut nulla provident et cumque minus. Ut recusandae quia est maxime nesciunt <strong>Ut repudiandae et ullam similique sed ducimus beatae est tenetur maxime</strong> non internos fugit. </p>

    <h2>Non reprehenderit voluptas et vero numquam et temporibus quaerat. </h2>
    <p>Sit placeat unde <em>Eum quae et quasi ullam sed praesentium quasi</em> qui dolores pariatur ut inventore reiciendis. Vel perspiciatis voluptateQuo deserunt ut blanditiis iusto qui quaerat omnis. In quisquam minima <strong>Nam ducimus et nihil dolores et magni velit</strong> non quas dicta? </p>

    <h3>How hiring me as an obituary writer will work. </h3>
    <p>You'll get in touch, telling me who the obituary is for, and how fast you need it. My contact info is linked at the top of the page.</p>
    
    <p>From there we'll schedule a time for a 30 minute phone call. During this chat you'll tell me all about your loved one's life, their personality, and any important details or anecdotes that capture their essence and arc of life. I'll send you a fully written obituary within about a week of our call.</p> 
    
    <p>After you've received my drafted obituary, you'll hav ethe opportunity to provide me with feedback and any edits you'd like to make. Once you're happy with the finished product, we can proceed with payment of <strong>$300</strong>, payable by Zelle or Venmo.</p>
    
    <p>Recounting the life of a loved one is difficult, but I hope to make this process as gentle and joyful as possible. </p>
  </div>
</div>
