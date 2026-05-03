---
layout: default
title: Beta Testing (TestFlight)
published: true
---

<img src="{{ '/assets/images/hero-banner.jpg' | relative_url }}" alt="Because nature isn't always accommodating" style="width:100%;border-radius:8px;margin-bottom:1.5rem;">

<div class="support-site-header">
  <nav class="lang-switch" aria-label="Language">
    <a href="{{ '/testflight.html' | relative_url }}" class="lang-switch__link" aria-current="page">English</a>
    <span class="lang-switch__sep" aria-hidden="true">·</span>
    <a href="{{ '/jp/testflight.html' | relative_url }}" class="lang-switch__link">日本語</a>
  </nav>
  <nav class="home-link-nav" aria-label="Site">
    <a href="{{ '/' | relative_url }}" class="home-link">Home</a>
  </nav>
</div>

# Thermal Buddy iOS — Beta Testing — TestFlight

<p class="page-meta">Thank you for helping make Thermal Buddy better.</p>

---

## From One Hiker to Another

You know the feeling.

You're lying in your tent at 2 a.m., staring at the ceiling. You've already pulled on every piece of clothing you packed, and you're still cold. You got the layering wrong — again.

Or maybe it's the morning before a big trip. You're going through your gear pile and thinking: *"Last year I did a similar route in October... was I too cold at camp? Did I bring the puffy? Was it enough?"* And you genuinely can't remember.

That's exactly what Thermal Buddy is for.

I built this app because I kept making the same layering mistakes. After enough cold nights and sweaty descents, I started writing things down. Temperature, what I wore, how I actually felt — scene by scene. When I had a few months of history, I realized how useful it was to search back and ask *"what gear worked for me in these exact conditions?"* And then the next trip got a little better. And the next one after that.

This beta is your chance to kick the tires before the public launch. You're not just a tester — you're the kind of person who cares enough about their gear to track it, and that makes your feedback uniquely valuable.

I'm looking forward to hearing what you think.

— Eiji

<a href="mailto:eiji@thermalbuddy.app" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;"><svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="flex-shrink:0;"><rect x="2" y="4" width="20" height="16" rx="2"/><polyline points="2,4 12,13 22,4"/></svg><span>eiji@thermalbuddy.app</span></a>

<a href="https://www.instagram.com/ultralight_for_espresso/" style="display:inline-flex;align-items:center;gap:6px;text-decoration:none;"><svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="flex-shrink:0;"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg><span>@ultralight_for_espresso</span></a>

---

## What Feedback Would Help Most

Picture these two scenarios as you explore the app — no real trip needed. Just imagine them as you tap through.

### 1. Logging After an Outing

You're back at camp or at the trailhead. You want to record what you wore.

- **Active scene:** what you had on while moving — hiking, running, scrambling.
- **Rest or Sleep scene:** what you added or swapped when you stopped — especially that tent moment at night.

*Did you feel too hot? Too cold? Just right?* Log it while the memory is fresh.

**Feedback I'm looking for:**
- Was the flow for adding a Sleep scene intuitive, or did something feel off?
- Did the gear categories match how you actually think about your kit?
- Was there anything you wanted to record that the app didn't have a field for?

### 2. Planning Your Next Trip

Now imagine you're preparing for your next outing. You open Search and ask: *"What did I wear for a Sleep scene around 5–10 °C?"*

Look at the results. Are they what you expected? Does seeing your own history help you decide what to pack?

**Feedback I'm looking for:**
- Does the Search result make you more confident about your gear choice — or does something feel confusing?
- Is there a planning question you wish the app could answer, but currently can't?
- Did a past log make you think *"oh right, I should bring that"* — or the opposite?

Anything that makes you think *"this would be so much better if…"* — that's exactly what I want to hear.

---

## Tips Before You Start

### Customise your activities and gear categories first

Before logging your first trip, it is worth spending a minute in **Settings** to tailor the app to how you actually think about your gear. You can rename, hide, reorder, or add custom activities and gear categories. For activities you can also change the icon. Getting this right upfront means every log you write after that will feel natural and quick.

### Tap a suggestion to fill in brand and category automatically

When adding a gear item, start typing in the item name field. If you have logged that piece of gear before, it will appear as a suggestion. Tap it and the brand and category fill in automatically — no need to type them at all.

---

## Developer Menu (Testing Tools)

The app includes a hidden set of developer tools to help you populate it with sample data quickly. This is intended for testers.

### How to Unlock

1. Open the app and go to **Settings** (the gear icon, last tab).
2. Scroll to the bottom of the Settings screen to find the **About** section.
3. Tap the **Build** row **5 times** in quick succession.
4. You will feel a haptic confirmation and a new **Data** section will appear above About.

To lock the developer tools again, tap the Build row 5 times once more.

### Loading Sample Data

Inside the **Data** section, you will find two buttons:

| Button | What it loads |
|--------|--------------|
| **Load App Store Data (EN)** | A set of English-language sample logs designed to showcase the Search feature. Good starting point for exploring the app. |
| **Load App Store Data (JA)** | The same set in Japanese. |

Tap either button to confirm the load. The sample logs will appear in your Logbook immediately.

### ⚠️ Warning: "Clear All Logs" Deletes Everything

The **Clear All Logs** button removes **every single log on your device** — including any real logs you have recorded yourself — not just the sample data. This action cannot be undone.

If you want to remove only the sample data, delete those entries manually from the Logbook (swipe left on a card to delete it).

---

## What's new in Build 6

- ✅ **Confirmation before discarding edits** — If you try to close a scene while there are unsaved changes, the app now asks what you want to do first. You can save your work or discard on purpose. The goal is fewer accidental losses of carefully entered details from a mistaken tap.

---

## What's new in Build 5

All of the improvements that were listed as "coming soon" in the previous build are now live.

- ✅ **Temperature picker** — you can now set both values to the same temperature, and pushing one side past the other moves the opposite side with it instead of snapping back.
- ✅ **Long press to type a temperature** — the centre of the wheel now requires a long press to open the keyboard, eliminating accidental triggers while scrolling.
- ✅ **Gear suggestions across scenes** — gear entered in an earlier scene during the same session now appears as an autofill suggestion in later scenes.
- ✅ **Smarter gear name matching** — suggestions now match anywhere within an item name, not only from the start. Prefix matches still appear first.
- ✅ **Brand-based gear suggestions** — typing a brand name surfaces gear from that brand in your history, before you start typing the item name.
- ✅ **Edit gear items in place** — tap any gear item to update its name, brand, or category directly. Works both during log creation and later in the Logbook.

See the full [Roadmap](roadmap.md) for what is coming next.

---

## Join the Beta on TestFlight

Follow these steps in order:

1. **Install the TestFlight app** from the App Store if you haven't already. ([Get TestFlight](https://apps.apple.com/app/testflight/id899247664))
2. **Tap the button below** (or tap it on your iPhone directly). Do not open the TestFlight app manually — tap the link first.
3. TestFlight will open automatically and show the Thermal Buddy beta.
4. Tap **Install** to download the app.

<p class="cta-actions"><a href="https://testflight.apple.com/join/q2s2cH73" class="github-issue-button" style="font-size:18px;padding:14px 30px;">Open in TestFlight</a></p>

> **If you see a "Ready to Test" screen with a "Redeem" or "Use Code" button**, you opened the TestFlight app directly instead of tapping the link above. Go back, and tap the button above — it will take you straight to the Thermal Buddy beta without needing a code.

> **No charges during the beta.** Any Premium purchases made through TestFlight use Apple's sandbox environment — your payment method will never be billed.
>
> **Beta duration.** I'm planning to run the beta for a few weeks. When it ends, TestFlight will notify you automatically.

---

## Questions?

Check the [Frequently Asked Questions (FAQ)](faq.md) — it covers how the app works in detail.

If you run into a bug or want to request a feature, please [open a GitHub Issue](https://github.com/nicola-vibecoder/thermal-buddy/issues). It's the fastest way to make sure it gets tracked.

---
{{ site.copyright }}
