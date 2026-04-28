---
layout: default
title: Home
---

<div class="support-page-banner">
<img src="{{ '/assets/images/banner-light-grey.svg' | relative_url }}" alt="Thermal Buddy" width="1536" height="1024" style="width:100%;max-width:100%;height:auto;display:block;margin:0 0 1.25rem 0;border-radius:4px;" />
</div>

# Welcome to Thermal Buddy Support

Thermal Buddy is a native iOS app created by Eiji, a hiker, backpacker, and trail runner who wanted a better way to remember what gear actually worked in real conditions. After each outing, you record temperature, scene, gear, and how you felt, then use your own history to plan what to wear next time. The benefit is practical and personal: fewer layering mistakes, more consistent comfort, and more confidence before your next trip.

## Support Resources

- [Frequently Asked Questions (FAQ)](faq.md)
- [Privacy Policy](privacy.md)
- [日本語ページはこちら (Japanese)](./jp/)

## Getting Help

The best way to get help or suggest features is to **[open an issue on our GitHub repository](https://github.com/nicola-vibecoder/thermal-buddy/issues)**.

Using GitHub Issues is the preferred method because:
- **Transparency:** You can see if others have reported the same issue.
- **Searchable:** Solutions become a public resource for the entire community.
- **Efficiency:** It helps me track and prioritize improvements directly in the codebase.

## Contact Us

If you have trouble using GitHub or have a private matter, use the buttons below to send an email. This method helps protect against automated spam.

<style>
.contact-button {
  display: inline-block;
  padding: 10px 20px;
  background-color: #24292e;
  color: #ffffff !important;
  text-decoration: none !important;
  border-radius: 6px;
  font-weight: 600;
  font-size: 14px;
  border: none;
  cursor: pointer;
  margin-top: 10px;
  transition: background-color 0.2s ease;
}
.contact-button:hover {
  background-color: #2f363d;
}
.contact-label {
  display: block;
  font-weight: 600;
  margin-top: 15px;
  margin-bottom: 5px;
}
</style>

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
{{ site.copyright }}
