---
layout: page
title: Contact
permalink: /contact/
priority: 4
---


<form name="contact" netlify-honeypot="b0tz" action="/thanks.html" netlify>
  <div class="row">
    <div class="column">
      <label for="name">Name</label>
      <input type="text" name="name" />
      <label for="email">Email</label>
      <input type="email" name="email" />
      <label for="subject">Subject</label>
      <input type="text" name="subject" />
      <p style="display:none;"><label><input name="b0tz"></label></p>
      <label for="message">Message</label>
      <textarea name="message" rows="8"></textarea>
      <p><button type="submit">Send</button></p>
    </div>
  </div>
</form>
