---
layout: page
title: Contact
permalink: /contact
priority: 4

twitter_username: ahannahseo
bluesky_username: hannahseo.com
instagram_username: v4nity_pl8
---

<div class="row pad-top">
  <div class="column left-rail">
    <h3>
      Find Hannah on <a href="https://twitter.com/{{ page.twitter_username }}">Twitter</a>, <a href="https://bsky.app/profile/{{ page.bluesky_username }}">Bluesky</a>, <a href="https://instagram.com/{{ page.instagram_username }}">Instagram</a>, and <a href="https://collageclub.substack.com">Collage Club</a>.
    </h3>
  </div>
  <div class="column">
    <form id="contact" name="contact" action="/thanks.html" netlify netlify-honeypot="botz">
      <div class="row">
        <div class="column">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" required />
        </div>
        <div class="column">
          <label for="email">Email</label>
          <input type="email" id="email" name="email" required />
        </div>
      </div>
      <div class="row">
        <div class="column">
          <label for="subject">Subject</label>
          <input type="text" id="subject" name="subject" />
          <p style="display:none;"><label><input id="b0tz" name="b0tz"></label></p>
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="8" required></textarea>
          <p><button type="submit">Send</button></p>
        </div>
      </div>
    </form>
  </div>
</div>
