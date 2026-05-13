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

- **Built for Hikers, by a hiker** - from real trail experience to solve real layering mistakes.
- **Practical & Personal**: Move beyond generic charts; rely on your own unique comfort levels.

<div class="app-store-cta" style="margin: 2rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">Try it Free on the App Store</a>
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
    <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">Try it Free on the App Store</a>
  </div>
</div>



<div class="sidebar-resources">
  <p class="view">
    <strong>Menu</strong>
    {% include nav-links-only.html %}
  </p>
</div>

---
{% include site-footer.html %}
