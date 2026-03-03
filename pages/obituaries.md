---
permalink: /obituaries
layout: page
nav_exclude: true
title: Professional Obituary Writing Services
description: "Hire Hannah Seo, a journalist and poet, to craft a narrative obituary that honors your loved one's life. $300 flat, includes phone consultation and revisions."
heading: Obituary Writing Services
contact_link: /contact
---

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Service",
  "name": "Custom Obituary Writing",
  "description": "Personalized narrative obituaries crafted to honor your loved one's life and personality.",
  "provider": {
    "@type": "Person",
    "name": "Hannah Seo",
    "url": "https://hannahseo.com"
  },
  "offers": {
    "@type": "Offer",
    "price": "300",
    "priceCurrency": "USD"
  },
  "url": "https://hannahseo.com/obituaries"
}
</script>

<div class="row pad-top">
  <div class="column">

    <h2>Let me help you honor the life of your loved one with a specially crafted obituary.</h2>

    <p>As a journalist, poet, and writer, I've had the honor of writing numerous obituaries for grieving families searching for a way to tell their loved one's life story.</p>

    <p>Nothing is worse than a bland obituary that fails to convey the unique and lively colors of a life once lived. With every obituary, I strive to get to every individual's essence, and to convey their life and personality with the love and vibrancy that their loved ones would like to remember them by. </p>

    <p>Whether you're seeking an obituary for a parent, spouse, or even for yourself — a <em>living obituary</em>, written while you're still here to shape your own story — I will craft a unique narrative obituary that captures their personality and honors their life.</p>

    <h3>How it works</h3>
    <ol>
      <li><strong>Get in touch.</strong> Reach out with who the obituary is for and how quickly you need it. My contact info is available above. </li>
      <li><strong>We talk.</strong> We'll schedule a 30-minute phone call where you tell me all about your loved one's life, their personality, and any important details and  anecdotes that capture their essence and arc of life.</li>
      <li><strong>I write, you review.</strong> I'll send you a fully written obituary within about a week of our call. From there, share your feedback and any edits you'd like to make until you're happy with the finished piece.</li>
      <li><strong>Payment.</strong> Once you're happy with the finished product, we can proceed with payment.</li>
    </ol>

    <h3>Details</h3>
    <ul>
      <li><strong>Price:</strong> $300 flat</li>
      <li><strong>Turnaround:</strong> ~1 week from our call</li>
      <li><strong>Includes:</strong> Phone consultation and revisions</li>
      <li><strong>Payment:</strong> Zelle or Venmo, due after approval</li>
    </ul>

    <p>Recounting the life of a loved one is difficult, but I hope to make this process as gentle and joyful as possible.</p><p></p>

  </div>

  <div class="column left-rail">
    <div>
      <h2><a href="{{page.contact_link}}"><u>Contact me here</u>.</a></h2>
    </div>

    <h3 class="pad-top">Testimonials</h3>
    <p>While I cannot publicly publish past obituaries I've written - out of respect for privacy - I am happy to share anonymized examples on request. In the meantime, below are a couple reviews from families I have worked with in the past.</p>

    {% for t in site.data.obit_t %}
    <div class="testimonial">
      <h4>
        "{{t.title}}"
      </h4>
      <p><em>{{t.body}}</em></p>
      <p>— {{t.name}}, {{t.date}}</p>
    </div>
    {% endfor %}
  </div>
</div>
