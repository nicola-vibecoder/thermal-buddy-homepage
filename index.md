---
layout: default
title: Home
move_nav_to_bottom: true
hide_site_header: true
---


# Stop Guessing.<br>Hike Warm. Sleep Warm.

Your past outings hold the answer. Thermal Buddy turns your hiking and camping logs into a personal comfort database — so you know exactly what to wear and carry before you ever leave the trailhead.

<div class="app-store-cta" style="margin: 2rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">Pack Right. Stay Warm. Download Free.</a>
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
      <img src="./assets/images/campaign-1.png?v=2" alt="Experience — No More Guesswork" class="carousel-slide">
      <img src="./assets/images/campaign-2.png?v=2" alt="Record — Every Skin Sensation" class="carousel-slide">
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

### Imagine Waking Up Warm Every Time

That's not luck — it's data. Thermal Buddy builds your personal comfort profile from real outings, so you stop packing by instinct and start packing by evidence.

- **ENJOY**: Know before you go. Pull up your logs and see exactly what worked in the same conditions — temperature, weather, terrain. No more second-guessing your sleep system at 2am.
- **REFINE**: Each outing sharpens your profile. Your data tells you what layer to keep, what to cut, and what to swap.
- **RECORD**: After each outing, log your layers, the conditions, and how you felt. Hot, cold, or Just Right. Takes 60 seconds.

### Why Thermal Buddy?

- **Built for Hikers. By a Hiker.** Eiji built this app after too many cold, sleepless nights under a tarp. It solves the layering and gear guessing game for good.
- **Your 'Just Right' is Unique.** Move beyond generic recommendations. Rely on your own comfort data — there's no one-size-fits-all when it comes to thermal comfort.

<div class="app-store-cta" style="margin: 3rem 0;">
  <a href="https://apps.apple.com/app/apple-store/id6764351164?pt=128836898&ct=Support%20Page%20Link&mt=8" class="app-store-button" onclick="zaraz.track('APPSTORE_CLICK');">Pack Right. Stay Warm. Download Free.</a>
</div>
<div class="sidebar-resources">
  <p class="view">
    <strong>Menu</strong>
    {% include nav-links-only.html %}
  </p>
</div>

---
{% include site-footer.html %}
