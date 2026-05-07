---
layout: default
title: Home
move_nav_to_bottom: true
---


# Welcome to Thermal Buddy

### How Thermal Buddy works

- **Record**: After your run or hike, log the temperature, wear + gear, and your actual skin sensation.
- **Build**: Create your personal database of what worked and what didn't in real conditions.
- **Plan**: No more guessing. Use your history to dial in the perfect layering for your next adventure.

### Why Thermal Buddy?

- Built for Hikers, by a hiker - from real trail experience to solve real layering mistakes.
- **Practical & Personal**: Move beyond generic charts; rely on your own unique comfort levels.

<style>
.campaign-carousel {
  position: relative;
  width: 100%;
  max-width: 380px;
  margin: 1.5rem auto 0;
  user-select: none;
}
.carousel-track-wrapper {
  overflow: hidden;
  border-radius: 16px;
}
.carousel-track {
  display: flex;
  transition: transform 0.45s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  will-change: transform;
  cursor: grab;
}
.carousel-track:active { cursor: grabbing; }
.carousel-slide {
  min-width: 100%;
  width: 100%;
  display: block;
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
  <div class="carousel-track-wrapper">
    <div class="carousel-track" id="carouselTrack">
      <img src="./assets/images/campaign-1.png" alt="Experience — No More Guesswork" class="carousel-slide">
      <img src="./assets/images/campaign-2.png" alt="Record — Every Skin Sensation" class="carousel-slide">
      <img src="./assets/images/campaign-3.png" alt="Refine — Find Your Perfect Setup" class="carousel-slide">
    </div>
  </div>
  <div class="carousel-dots" id="carouselDots">
    <button class="carousel-dot active" aria-label="Slide 1" onclick="tbCarousel.go(0)"></button>
    <button class="carousel-dot" aria-label="Slide 2" onclick="tbCarousel.go(1)"></button>
    <button class="carousel-dot" aria-label="Slide 3" onclick="tbCarousel.go(2)"></button>
  </div>
</div>

<script>
(function () {
  var track = document.getElementById('carouselTrack');
  var dotEls = document.querySelectorAll('#carouselDots .carousel-dot');
  var current = 0;
  var total = 3;
  var startX = 0;
  var dragging = false;
  var timer;

  function go(idx) {
    current = ((idx % total) + total) % total;
    track.style.transform = 'translateX(-' + (current * 100) + '%)';
    dotEls.forEach(function (d, i) { d.classList.toggle('active', i === current); });
  }

  function resetTimer() {
    clearInterval(timer);
    timer = setInterval(function () { go(current + 1); }, 4000);
  }

  window.tbCarousel = {
    go: function (idx) { go(idx); resetTimer(); }
  };

  track.addEventListener('touchstart', function (e) { startX = e.touches[0].clientX; dragging = true; }, { passive: true });
  track.addEventListener('touchend', function (e) {
    if (!dragging) return;
    var diff = startX - e.changedTouches[0].clientX;
    if (Math.abs(diff) > 40) { go(diff > 0 ? current + 1 : current - 1); resetTimer(); }
    dragging = false;
  }, { passive: true });

  track.addEventListener('mousedown', function (e) { startX = e.clientX; dragging = true; });
  track.addEventListener('mouseup', function (e) {
    if (!dragging) return;
    var diff = startX - e.clientX;
    if (Math.abs(diff) > 40) { go(diff > 0 ? current + 1 : current - 1); resetTimer(); }
    dragging = false;
  });
  track.addEventListener('mouseleave', function () { dragging = false; });

  resetTimer();
})();
</script>

<div class="app-store-cta">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('App Store Clicked')">Start Free Trial on App Store</a>
</div>

<div class="sidebar-resources">
  <p class="view">
    <strong>Menu</strong>
    {% include nav-links-only.html %}
  </p>
</div>

---
{% include site-footer.html %}
