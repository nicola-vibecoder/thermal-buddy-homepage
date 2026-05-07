---
layout: default
title: お問い合わせ
---


# お問い合わせ

GitHub の利用が難しい場合や、個別の連絡が必要な場合は以下のボタンからメールを送信してください。スパム対策としてメールアドレスを保護しています。

<script>
function sendSecureEmail(encodedEmail) {
  window.location.href = 'mailto:' + atob(encodedEmail);
}
</script>

<div class="contact-label">サポート (技術的な問題など)</div>
<button class="contact-button" onclick="sendSecureEmail('c3VwcG9ydEB0aGVybWFsYnVkZHkuYXBw')">サポートへメールを送信</button>

<div class="contact-label">一般のお問い合わせ (取材・ビジネスなど)</div>
<button class="contact-button" onclick="sendSecureEmail('aW5xdWlyeUB0aGVybWFsYnVkZHkuYXBw')">お問い合わせメールを送信</button>

---
{% include site-footer.html %}
