---
layout: default
title: Contact Us
---


# Contact Us

If you have trouble using GitHub or have a private matter, use the buttons below to send an email. This method helps protect against automated spam.

<script>
function sendSecureEmail(encodedEmail) {
  window.location.href = 'mailto:' + atob(encodedEmail);
}
</script>

<div class="contact-label">Support (Technical Issues)</div>
<button class="contact-button" onclick="sendSecureEmail('c3VwcG9ydEB0aGVybWFsYnVkZHkuYXBw')">Send Email to Support</button>

<div class="contact-label">General Inquiries (Press/Business)</div>
<button class="contact-button" onclick="sendSecureEmail('aW5xdWlyeUB0aGVybWFsYnVkZHkuYXBw')">Send General Inquiry</button>

---
{% include site-footer.html %}
