---
layout: default
title: Roadmap
---

{% include site-banner-lang.html %}

# Roadmap

<p class="page-meta">Last updated: May 2026</p>

This page shares what we are currently working on and what we are thinking about next. Nothing here is a firm promise — real-world development has a way of surprising everyone — but it reflects where our heads are right now.

If something on this page matters to you, or if something important is missing entirely, please [open a GitHub issue](https://github.com/nicola-vibecoder/thermal-buddy/issues) and let us know. Your feedback shapes what gets prioritised.

---

## Coming in upcoming releases

These are the improvements we are actively working on. Our goal is to get them into your hands as quickly as possible.

### Temperature picker improvements

Setting a temperature range should feel effortless. Right now there are a couple of rough edges: you cannot set both the minimum and maximum to the same value, and if you push one side past the other it snaps back unexpectedly instead of moving the other side along with it. We are smoothing both of these out so the picker behaves the way you would naturally expect.

### Long press to type a temperature

Tapping the centre of the temperature wheel currently opens a keyboard for direct number entry — a useful shortcut, but too easy to trigger accidentally while simply scrolling. We are changing it to a deliberate long press so you can spin the wheel freely without unexpected interruptions. A small on-screen hint will let you know the shortcut is there.

### Gear suggestions that work across your whole session

When you are logging a trip with multiple scenes back to back, gear you added to an earlier scene in the same session should appear as autofill suggestions when you add gear to a later one. We are improving this so your entire in-progress log counts as a suggestion source — not just the scene you are editing right now.

### Smarter gear name suggestions

Typing part of a gear item name currently only matches from the beginning — so "Tights" would not surface "Light Alpha Tights" from your history. We are improving this so that matches within the name also count, making it easier to find items you have logged before. Exact prefix matches will still appear first.

### Suggestions based on the brand you type

Once you type a brand name, Thermal Buddy will start suggesting gear items from that brand that appear in your log history — even before you have begun typing the item name. Less retyping, faster logging.

### Fix typos in gear without deleting and starting over

Added a gear item and noticed a typo in the name, or picked the wrong category? Right now the only way to fix it is to delete the item and add it again from scratch — frustrating when you just want to correct one letter. We are adding in-place editing so you can tap any gear item, either while you are still creating the log or later in your logbook, and adjust the name, brand, or category without losing anything.

---

## Thinking about — your feedback welcome

The items below are ideas we find interesting but have not yet committed to building. Before investing the time, we would love to know whether they would actually be useful to you.

**If any of these would make a meaningful difference to how you use the app, please tell us via [GitHub Issues](https://github.com/nicola-vibecoder/thermal-buddy/issues).** We read every submission.

### Notes on individual gear items

A small free-text notes field attached to each piece of gear — for details like "wore this as a mid-layer only" or "borrowed, not mine." Notes would appear when reviewing a past scene in your logbook.

### Choose the order of your scene types

Active, Rest, Sleep, and Transit always appear in the same fixed order across the app. A future option could let you rearrange them so the scenes you use most often appear first.

### My Gear — a quick view of everything you have logged

A dedicated screen listing all the gear that has ever appeared in your logs, organised by category, so you can get a quick overview of your kit without opening individual trip records.

### Adjust how cautious Search is about cold

The Search screen already treats cold-side gaps as twice as serious as warm-side gaps, because getting colder than expected in the outdoors carries more real risk. A future setting could let you tune this balance up or down to match your personal comfort with risk.

---

## Not on the roadmap

Ideas we have considered but decided not to pursue for now. We may revisit any of these if the situation changes.

*Nothing to list yet — watch this space.*

---

{{ site.copyright }}
