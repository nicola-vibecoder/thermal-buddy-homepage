---
layout: default
title: ホーム
---

{% include site-banner-lang.html %}

# Thermal Buddy サポートへようこそ

Thermal Buddy は、ハイカー・バックパッカー・トレイルランナーでもある Eiji が、「実際のコンディションで何を着て快適だったか」を振り返れるように作ったネイティブ iOS アプリです。山行後に気温・シーン・着用ギア・体感を記録し、次回の山行で何を着るべきかを自分の履歴から判断できます。レイヤリングの失敗を減らし、快適性を安定させ、出発前の判断に自信を持てるのがメリットです。

## サポートリソース

- [よくある質問 (FAQ)](faq.md)
- [プライバシーポリシー](privacy.md)

## ヘルプが必要な場合

バグの報告や機能の提案には、**[GitHub リポジトリで Issue を作成する](https://github.com/nicola-vibecoder/thermal-buddy/issues)** のが最も確実な方法です。

GitHub での報告を推奨する理由は以下の通りです。
- **透明性:** 他のユーザーが同じ問題を報告していないか確認できます。
- **ナレッジ共有:** 解決した内容が、将来的に他のユーザーの助けになります。
- **迅速な対応:** 開発者が直接、効率的に機能追加や修正を管理・優先順位付けできます。

## お問い合わせ

GitHub の利用が難しい場合や、個別の連絡が必要な場合は以下のボタンからメールを送信してください。スパム対策としてメールアドレスを保護しています。

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

<div class="contact-label">サポート (技術的な問題など)</div>
<button class="contact-button" onclick="sendSecureEmail('c3VwcG9ydEB0aGVybWFsYnVkZHkuYXBw')">サポートへメールを送信</button>

<div class="contact-label">一般のお問い合わせ (取材・ビジネスなど)</div>
<button class="contact-button" onclick="sendSecureEmail('aW5xdWlyeUB0aGVybWFsYnVkZHkuYXBw')">お問い合わせメールを送信</button>

---
{{ site.copyright }}
