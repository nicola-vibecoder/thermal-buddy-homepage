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

## Shipped in Build 7

### ✅ My Gear

A dedicated screen listing all the gear you have ever logged, organised by category. You can search, sort by category, brand, or name, and tap any item to see its full log history — every trip it has appeared in, with a direct link to each log's detail view.

You can also add gear to your catalog before a trip, without needing to create a log first. Items that have not yet appeared in any log are marked clearly so you know they are catalog-only entries.

Every stat tile on the Home screen is now tappable: Outings takes you straight to the Logbook, Just Right % shows a filtered view of your well-matched logs, and My Gear opens the new gear list.

### ✅ Duplicate a log

You can now duplicate any existing log from the Logbook. Swipe left on a card or open a log and use the toolbar button to create a copy, which opens immediately in edit mode ready for you to adjust. Free plan limits apply.

---

## Shipped in Build 6

### ✅ Confirmation before discarding edits

If you try to close a scene while there are unsaved changes, the app now asks what you want to do first. You can save your work or discard on purpose. The goal is fewer accidental losses of carefully entered details from a mistaken tap.

---

## Shipped in Build 5

Everything that was listed as "coming soon" in the previous build has now landed. Here is what is new.

### ✅ Temperature picker improvements

You can now set the minimum and maximum temperature to the same value, and pushing one side past the other moves the opposite side along with it instead of snapping back. The picker behaves the way you would naturally expect.

### ✅ Long press to type a temperature

The centre of the temperature wheel now requires a deliberate long press to open the keyboard for direct number entry. Accidental triggers while scrolling no longer happen. A small on-screen hint lets you know the shortcut is there.

### ✅ Gear suggestions across your whole session

When logging a trip with multiple scenes, gear you entered in an earlier scene now appears as an autofill suggestion in later scenes within the same session. Your entire in-progress log counts as the suggestion source.

### ✅ Smarter gear name suggestions

Suggestions now match anywhere within a gear item name — so typing "Tights" will surface "Light Alpha Tights" from your history. Prefix matches still appear first.

### ✅ Suggestions based on the brand you type

Once you type a brand name, Thermal Buddy surfaces gear items from that brand in your log history, before you have even started typing the item name.

### ✅ Fix typos in gear without deleting and starting over

You can now tap any gear item — both while creating a log and later in the Logbook — and edit its name, brand, or category in place. No more deleting and re-adding just to fix one letter.

---

## Coming in upcoming releases

We are currently heads-down on stability and polish. No major features are in active development right now. Watch this space.

---

## Thinking about — your feedback welcome

The items below are ideas we find interesting but have not yet committed to building. Before investing the time, we would love to know whether they would actually be useful to you.

**If any of these would make a meaningful difference to how you use the app, please tell us via [GitHub Issues](https://github.com/nicola-vibecoder/thermal-buddy/issues).** We read every submission.

### Notes on individual gear items

A small free-text notes field attached to each piece of gear — for details like "wore this as a mid-layer only" or "borrowed, not mine." Notes would appear when reviewing a past scene in your logbook.

### Choose the order of your scene types

Active, Rest, Sleep, and Transit always appear in the same fixed order across the app. A future option could let you rearrange them so the scenes you use most often appear first.

### Adjust how cautious Search is about cold

The Search screen already treats cold-side gaps as twice as serious as warm-side gaps, because getting colder than expected in the outdoors carries more real risk. A future setting could let you tune this balance up or down to match your personal comfort with risk.

---

## Not on the roadmap

Ideas we have considered but decided not to pursue for now. We may revisit any of these if the situation changes.

*Nothing to list yet — watch this space.*

---

## Long-term dreams

These are things we genuinely hope to do someday, but have no timeline for. Consider them aspirations rather than plans.

### Android version

Thermal Buddy is iOS-only today. Building a great Android version is a real goal, but it requires rebuilding the app from the ground up — it is a significant undertaking and not something we can promise on any particular schedule.

### Spanish language support

We would love to make Thermal Buddy accessible to Spanish-speaking communities. If you are a native Spanish speaker who would be interested in helping with localisation, please do reach out via [GitHub Issues](https://github.com/nicola-vibecoder/thermal-buddy/issues).

---

{{ site.copyright }}
