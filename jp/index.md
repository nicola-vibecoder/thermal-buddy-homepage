---
layout: default
title: ホーム
move_nav_to_bottom: true
---


# Thermal Buddy へようこそ

### Thermal Buddy の使い方

- **RECORD**: ハイキングやランの後に、気温、天候、着用ウェア・ギア、そして「暑かった」「寒かった」「ちょうどよかった」という体感を記録します。
- **REFINE**: 実際のフィールドで「何がうまくいき、何がダメだったか」を自分だけのデータベースとして蓄積します。
- **ENJOY**: もう勘に頼らない。データを使って、次の山行に最適なレイヤリングやスリーピングギアを導き出しましょう。あとは、ただアウトドア体験を楽しむだけです。

### なぜ Thermal Buddy？

- **ハイカーが、ハイカーのために作った**: バックパッカーでありトレイルランナーでもある開発者のEijiが、タープの下で何度も寒さに震え、眠れない夜を過ごした経験からこのアプリを作りました。「勘」に頼ったウェアやスリーピングギア選びの失敗 - あの「寒い」失敗 - を何度も繰り返さないために。
- **あなたの「ちょうどいい」は、あなただけのもの**: あなた自身の「快適」を基準にしましょう。快適な体感温度に「万人向け」の正解はありません。
- **高いカスタマイズ性**: どんなアウトドアアクティビティでも、Thermal Buddyは対応します。アクティビティ、シーン、ギアカテゴリーを自由にカスタマイズして、あなたが必要とするデータだけを記録できます。アイコンもあなた好みに変更できます。

<div class="app-store-cta" style="margin: 2rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">App Store で無料で試す</a>
</div>

<style>
.campaign-carousel {
  position: relative;
  width: 90%;
  max-width: 342px;
  margin: 1.5rem auto 0;
  user-select: none;
}
.carousel-track-wrapper {
  overflow-x: scroll;
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  border-radius: 16px;
  scrollbar-width: none;
  -ms-overflow-style: none;
}
.carousel-track-wrapper::-webkit-scrollbar { display: none; }
.carousel-track {
  display: flex;
}
.carousel-slide {
  min-width: 100%;
  width: 100%;
  display: block;
  scroll-snap-align: start;
  border-radius: 16px;
  pointer-events: none;
}
.carousel-dots {
  display: flex;
  justify-content: center;
  gap: 10px;
  margin-top: 14px;
}
.carousel-dot {
  width: 8px;
  height: 8px;
  border-radius: 50%;
  border: none;
  background: #d1d5db;
  cursor: pointer;
  padding: 0;
  transition: background 0.2s, transform 0.2s;
}
.carousel-dot.active {
  background: #22C55E;
  transform: scale(1.3);
}
.carousel-dot:hover { background: #9ca3af; }
.carousel-dot.active:hover { background: #16a34a; }

.sticky-cta-container {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  box-sizing: border-box;
  background: rgba(255, 255, 255, 0.95);
  border-top: 1px solid #e5e7eb;
  padding: 1rem;
  box-shadow: 0 -4px 6px -1px rgba(0, 0, 0, 0.1);
  z-index: 1000;
  display: flex;
  justify-content: center;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
}
@media (min-width: 768px) {
  .sticky-cta-container {
    display: none;
  }
}
</style>

<div class="campaign-carousel">
  <div class="carousel-track-wrapper" id="carouselWrapper">
    <div class="carousel-track" id="carouselTrack">
      <img src="../assets/images/Campaign-JP1.png" alt="EXPERIENCE — No More Guesswork" class="carousel-slide">
      <img src="../assets/images/Campaign-JP2.png" alt="RECORD — Every Skin Sensation" class="carousel-slide">
      <img src="../assets/images/Campaign-JP3.png" alt="REFINE — Find Your Perfect Setup" class="carousel-slide">
    </div>
  </div>
  <div class="carousel-dots" id="carouselDots">
    <button class="carousel-dot active" aria-label="スライド 1" onclick="tbCarousel.go(0)"></button>
    <button class="carousel-dot" aria-label="スライド 2" onclick="tbCarousel.go(1)"></button>
    <button class="carousel-dot" aria-label="スライド 3" onclick="tbCarousel.go(2)"></button>
  </div>
</div>

<script>
(function () {
  var wrapper = document.getElementById('carouselWrapper');
  var dotEls = document.querySelectorAll('#carouselDots .carousel-dot');
  var current = 0;
  var total = 3;
  var timer;
  var scrollSettleTimer;

  function updateDots() {
    dotEls.forEach(function (d, i) { d.classList.toggle('active', i === current); });
  }

  function go(idx) {
    current = ((idx % total) + total) % total;
    wrapper.scrollTo({ left: current * wrapper.offsetWidth, behavior: 'smooth' });
    updateDots();
  }

  function resetTimer() {
    clearInterval(timer);
    timer = setInterval(function () { go(current + 1); }, 4000);
  }

  window.tbCarousel = {
    go: function (idx) { go(idx); resetTimer(); }
  };

  // Sync dots when user swipes natively
  wrapper.addEventListener('scroll', function () {
    clearTimeout(scrollSettleTimer);
    scrollSettleTimer = setTimeout(function () {
      var idx = Math.round(wrapper.scrollLeft / wrapper.offsetWidth);
      if (idx !== current) {
        current = idx;
        updateDots();
        resetTimer();
      }
    }, 80);
  }, { passive: true });

  resetTimer();
})();
</script>

<div class="sticky-cta-container">
  <div class="app-store-cta" style="margin: 0; width: 100%;">
    <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">App Store で無料で試す</a>
  </div>
</div>



<div class="sidebar-resources">
  <p class="view">
    <strong>メニュー</strong>
    {% include nav-links-only.html %}
  </p>
</div>

---
{% include site-footer.html %}
