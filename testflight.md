---
layout: default
title: Beta Testing (TestFlight)
published: false
---

{% include site-banner-lang.html %}

# Beta Testing — TestFlight

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

## Join the Beta on TestFlight

<p class="cta-actions"><a href="https://testflight.apple.com/join/q2s2cH73" class="github-issue-button">Open in TestFlight</a></p>

> **Note:** The TestFlight link will be active once Apple finishes reviewing the app. Check back soon.

---

## What Feedback Would Help Most

The two scenarios below are where I most want your honest reaction. Use them as your testing lens.

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

A few weeks later, you're preparing for another outing. You open Search and ask: *"What did I wear for a Sleep scene around 5–10 °C?"*

Look at the results. Are they what you expected? Does seeing your own history help you decide what to pack?

**Feedback I'm looking for:**
- Does the Search result make you more confident about your gear choice — or does something feel confusing?
- Is there a planning question you wish the app could answer, but currently can't?
- Did a past log make you think *"oh right, I should bring that"* — or the opposite?

Anything that makes you think *"this would be so much better if…"* — that's exactly what I want to hear.

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

## Questions?

Check the [Frequently Asked Questions (FAQ)](faq.md) — it covers how the app works in detail.

If you run into a bug or want to request a feature, please [open a GitHub Issue](https://github.com/nicola-vibecoder/thermal-buddy/issues). It's the fastest way to make sure it gets tracked.

---
{{ site.copyright }}
