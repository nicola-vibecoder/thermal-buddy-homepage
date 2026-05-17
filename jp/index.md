---
layout: default
title: ホーム
move_nav_to_bottom: true
hide_site_header: true
---


<h1 style="font-size: 1.5rem; line-height: 1.4; margin-bottom: 1rem;">もうレイヤリングに迷わない。<br>歩く時も、眠る時も快適に。</h1>

過去のアクティビティデータが答えを教えてくれます。Thermal Buddyは、あなたの山行記録から、あなただけの「快適データベース」を作ります。山に向けて出発する前に、何を着て、何を持っていくべきかが正確に分かります。

<div class="app-store-cta" style="margin: 2rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">寒くて眠れない夜にさよなら。<br>無料でダウンロード。</a>
</div>

<style>
.campaign-carousel {
  position: relative;
  width: 90%;
  max-width: 342px;
  margin: 1.5rem auto 2.5rem;
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
</style>

<div class="campaign-carousel">
  <div class="carousel-track-wrapper" id="carouselWrapper">
    <div class="carousel-track" id="carouselTrack">
      <img src="../assets/images/Campaign-JP1.png?v=2" alt="EXPERIENCE — No More Guesswork" class="carousel-slide">
      <img src="../assets/images/Campaign-JP2.png?v=2" alt="RECORD — Every Skin Sensation" class="carousel-slide">
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

### 朝までずっと暖かい、そんな体験を。

運ではなくデータに頼りましょう。Thermal Buddyは実際のフィールド体験からあなた専用の快適プロファイルを作成します。もう勘でパッキングするのはやめて、確かなデータに基づいた装備選びを始めましょう。

- **ENJOY (楽しむ)**: 行く前に分かる。過去のログを呼び出して、同じ条件（気温、天候、アクティビティ）で何がうまくいったかを正確に確認。夜中の2時にスリーピングシステムを後悔することはもうありません。
- **REFINE (洗練する)**: 一回のアクティビティごとにプロファイルが研ぎ澄まされる。データが「持っていくべきレイヤー」「外すべきギア」「交換すべきアイテム」を教えてくれます。
- **RECORD (記録する)**: 活動後、使ったウェア、スリーピングギア、コンディション、そして「暑い」「寒い」「ちょうどいい」といった体感を記録。簡単に記録できます。

### なぜ Thermal Buddy？

- **ハイカーが、ハイカーのために作りました** バックパッカーでありトレイルランナーでもあるEijiが、タープの下で何度も寒さに震え、眠れない夜を過ごした経験から作りました。ウェアやギア選びの「勘」に頼るのを止めるために。
- **あなたの「ちょうどいい」は、あなただけのもの** 一般的な推奨値から一歩先へ。あなた自身の快適データを信頼しましょう。体感温度に「万人向け」の正解はありません。

<div class="app-store-cta" style="margin: 3rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">もうパッキングに悩まない。<br>無料でダウンロード。</a>
</div>

<div class="sidebar-resources">
  <p class="view">
    <strong>メニュー</strong>
    {% include nav-links-only.html %}
  </p>
</div>

---
{% include site-footer.html %}
