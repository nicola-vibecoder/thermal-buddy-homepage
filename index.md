---
layout: default
title: Home
---

{% include site-banner-lang.html %}

# Welcome to Thermal Buddy Support

Thermal Buddy is a native iOS app created by Eiji, a hiker, backpacker, and trail runner who wanted a better way to remember what gear actually worked in real conditions. After each outing, you record temperature, scene, gear, and how you felt, then use your own history to plan what to wear next time. The benefit is practical and personal: fewer layering mistakes, more consistent comfort, and more confidence before your next trip.

## Support Resources

- [Frequently Asked Questions (FAQ)](faq.md)
- [Roadmap](roadmap.md)
- [Version History](version-history.md)
- [Privacy Policy](privacy.md)

## Getting Help

The best way to get help or suggest features is to open an issue on GitHub.

<p class="cta-actions"><a href="https://github.com/nicola-vibecoder/thermal-buddy/issues" class="github-issue-button">Open GitHub Issues</a></p>

Using GitHub Issues is the preferred method because:
- **Transparency:** You can see if others have reported the same issue.
- **Searchable:** Solutions become a public resource for the entire community.
- **Efficiency:** It helps me track and prioritize improvements directly in the codebase.

## Contact Us

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
{{ site.copyright }}
