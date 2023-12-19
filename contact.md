---
layout: page
title: Contact
permalink: /contact/
priority: 4
---

<div class="row">
  <div class="column left-rail">
    <h3>
      Find Hannah on <a href="https://twitter.com/{{ site.twitter_username }}">Twitter</a>, <a href="https://bsky.app/profile/{{ site.bluesky_username }}">Bluesky</a>, and <a href="https://www.instagram.com/{{ site.instagram_username }}">Instagram</a>.
    </h3>
  </div>
  <div class="column">
    <form name="contact" netlify-honeypot="b0tz" action="/thanks.html" netlify>
      <div class="row">
        <div class="column">
          <label for="name">Name</label>
          <input type="text" name="name" required />
        </div>
        <div class="column">
          <label for="email">Email</label>
          <input type="email" name="email" required />
        </div>
      </div>
      <div class="row">
        <div class="column">
          <label for="subject">Subject</label>
          <input type="text" name="subject" />
          <p style="display:none;"><label><input name="b0tz"></label></p>
          <label for="message">Message</label>
          <textarea name="message" rows="8" required></textarea>
          <p><button type="submit">Send</button></p>
        </div>
      </div>
    </form>
  </div>
</div>