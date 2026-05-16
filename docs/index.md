---
title: Home
hide:
  - toc
---

<style>
/* v1.9.1: Suppress the auto-injected page-section TOC inside the mobile drawer
   for the home page only. Material lifts each page's H2 section list into the
   primary drawer under the active page item AND exposes a chevron toggle (label
   for="__toc") that reveals "Table of contents → What is Meshtastic / Get
   Started / ..." on tap. Will reported this as junk UX on Home. Fix: hide the
   toggle label + chevron + secondary nav, and force the plain anchor (normally
   hidden on mobile when the toggle is present) back into view so the active
   "Home" row still renders. Scoped to Home only via inline <style> in
   docs/index.md — other pages retain their default in-drawer TOC chevron. */
.md-nav--primary .md-nav__item--active > label.md-nav__link[for="__toc"],
.md-nav--primary .md-nav__item--active > nav.md-nav--secondary,
.md-nav--primary .md-nav__item--active > input#__toc {
  display: none !important;
}
.md-nav--primary .md-nav__item--active > a.md-nav__link {
  display: flex !important;
}
</style>

<h1>Find Your Squad at Electric Forest — Without Cell Service.</h1>

Meshtastic is a tiny radio that clips to your pack and lets you text your friends across the Forest **even when cell service is dead**. No subscription. No SIM card. No monthly fee. About $30 to get on the mesh.

This is the community guide for using it at Electric Forest.

<div class="ef-phone-anim" aria-hidden="true">
  <div class="ef-phone">
    <svg class="ef-phone-frame" viewBox="0 0 240 480" xmlns="http://www.w3.org/2000/svg" preserveAspectRatio="xMidYMid meet" focusable="false">
      <rect x="2" y="2" width="236" height="476" rx="32" ry="32" fill="#1a0f33" stroke="#a78bfa" stroke-width="2"/>
      <rect x="10" y="10" width="220" height="460" rx="26" ry="26" fill="#15092b"/>
      <rect x="92" y="14" width="56" height="14" rx="7" fill="#0a0518"/>
    </svg>
    <div class="ef-phone-screen">
      <div class="ef-statusbar">
        <span class="ef-time">10:42</span>
        <span class="ef-carrier">EFMesh</span>
        <span class="ef-battery" aria-hidden="true">
          <svg viewBox="0 0 22 10" width="22" height="10"><rect x="0.5" y="0.5" width="18" height="9" rx="2" fill="none" stroke="#bda7f5" stroke-width="1"/><rect x="2" y="2" width="13" height="6" rx="1" fill="#b6f0a8"/><rect x="19.5" y="3" width="2" height="4" rx="0.5" fill="#bda7f5"/></svg>
        </span>
      </div>
      <div class="ef-chatheader">
        <span class="ef-meshicon" aria-hidden="true">
          <svg viewBox="0 0 24 24" width="16" height="16" fill="none" stroke="#b6f0a8" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><circle cx="5" cy="6" r="2"/><circle cx="19" cy="6" r="2"/><circle cx="12" cy="18" r="2"/><line x1="5" y1="6" x2="19" y2="6"/><line x1="5" y1="6" x2="12" y2="18"/><line x1="19" y1="6" x2="12" y2="18"/></svg>
        </span>
        <span class="ef-chattitle">EF Mesh &mdash; Squad Chat</span>
      </div>
      <div class="ef-chatbody">
        <div class="ef-msg ef-msg--in ef-msg--1"><span class="ef-name">alex</span><span class="ef-bubble">happy forest! where&rsquo;s the squad? &#127795;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--2"><span class="ef-name">sam</span><span class="ef-bubble">sherwood by the carousel &#127904;</span></div>
        <div class="ef-msg ef-msg--out ef-msg--3"><span class="ef-name">you</span><span class="ef-bubble">ranch arena in 10 &mdash; bring water &#128167;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--4"><span class="ef-name">jess</span><span class="ef-bubble">save me a spot &#128591;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--5"><span class="ef-name">alex</span><span class="ef-bubble">rain incoming, head back &#9748;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--6"><span class="ef-name">sam</span><span class="ef-bubble">battery dying find me later &#128267;</span></div>
        <div class="ef-msg ef-msg--out ef-msg--7"><span class="ef-name">you</span><span class="ef-bubble">drop a pin &#128205;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--8"><span class="ef-name">jess</span><span class="ef-bubble">this set is INSANE &#128293;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--9"><span class="ef-name">alex</span><span class="ef-bubble">happy forest &#127795; random wook just gave me kandi &#127752;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--10"><span class="ef-name">sam</span><span class="ef-bubble">forest fam heading to the observatory &#128301;</span></div>
        <div class="ef-msg ef-msg--out ef-msg--11"><span class="ef-name">you</span><span class="ef-bubble">wishing tree at midnight? &#127795;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--12"><span class="ef-name">jess</span><span class="ef-bubble">fam where r u im lost in sherwood lol</span></div>
        <div class="ef-msg ef-msg--in ef-msg--13"><span class="ef-name">alex</span><span class="ef-bubble">trading post in 30, rally up</span></div>
        <div class="ef-msg ef-msg--in ef-msg--14"><span class="ef-name">sam</span><span class="ef-bubble">vibe check &#10024; everyone safe?</span></div>
        <div class="ef-msg ef-msg--out ef-msg--15"><span class="ef-name">you</span><span class="ef-bubble">all good &mdash; happy forest &#128156;</span></div>
        <div class="ef-msg ef-msg--in ef-msg--16"><span class="ef-name">jess</span><span class="ef-bubble">headliner!! &#127926; see u at ranch arena</span></div>
      </div>
    </div>
  </div>
  <p class="ef-phone-caption">Real chats from your squad &mdash; no cell tower needed.</p>
</div>

<div class="stats-row" markdown>
<div class="stat"><span class="stat-num">120+</span><span class="stat-label">nodes last year</span></div>
<div class="stat"><span class="stat-num">15,000+</span><span class="stat-label">messages last year</span></div>
<div class="stat"><span class="stat-num">4</span><span class="stat-label">days of Forest</span></div>
</div>

<span style="display: flex; align-items: center; justify-content: center; gap: 1rem; flex-wrap: wrap; margin: 1.5rem 0;">
    [:fontawesome-brands-discord: Join EF Meshtastic on Discord](https://discord.com/channels/260909643574935553/1111482301730271232){ .md-button .md-button--primary target="_blank"}
    [:material-information-outline: New here? Start with How to Connect](docs/how-to-connect.md){ .md-button }
</span>

*Not in the Discord? Join at [discord.gg/electricforest](https://discord.gg/electricforest){ target=_blank } first.*{ .discord-helper }

---

## What is Meshtastic?

It's a little 915 MHz radio (about the size of a deck of cards or smaller) that:

- **Pairs to your phone over Bluetooth** so you can type messages on your phone screen
- **Sends texts + GPS locations to your squad** without any cell service or wifi
- **Meshes** — every node in the Forest extends the range for everyone else. The more of us, the better it works.

The little device connects via Bluetooth to your phone and lets you send messages and see each other's locations **without cell service**.

---

<div class="mesh-animation" aria-hidden="true">
<svg viewBox="0 0 600 280" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Mesh network animation showing 12 phones distributed across a festival camp, connected by dashed lines, with an orange message dot hopping between nodes">
  <defs>
    <symbol id="phone" viewBox="0 0 24 36">
      <rect x="2" y="2" width="20" height="32" rx="3" ry="3" fill="#2e1d4d" stroke="#a78bfa" stroke-width="1.5"/>
      <rect x="4" y="6" width="16" height="22" rx="1" fill="#7dd87a"/>
      <circle cx="12" cy="31" r="1.3" fill="#a78bfa"/>
    </symbol>
  </defs>
  <g class="mesh-links" stroke="#7dd87a" stroke-width="1" stroke-dasharray="3 3" opacity="0.4" fill="none">
    <!-- Cluster A — upper-left main camp (P1,P2,P3) -->
    <line x1="72"  y1="58"  x2="107" y2="93"/>
    <line x1="107" y1="93"  x2="142" y2="60"/>
    <line x1="72"  y1="58"  x2="142" y2="60"/>
    <!-- Cluster B — center stage area (P4,P5,P6) -->
    <line x1="247" y1="128" x2="282" y2="168"/>
    <line x1="247" y1="128" x2="322" y2="113"/>
    <line x1="282" y1="168" x2="322" y2="113"/>
    <!-- Cluster C — back camp lower-right (P7,P8,P9) -->
    <line x1="447" y1="193" x2="487" y2="223"/>
    <line x1="487" y1="223" x2="522" y2="183"/>
    <line x1="447" y1="193" x2="522" y2="183"/>
    <!-- Bridges between clusters + outliers -->
    <line x1="142" y1="60"  x2="402" y2="58"/>
    <line x1="402" y1="58"  x2="322" y2="113"/>
    <line x1="107" y1="93"  x2="187" y2="218"/>
    <line x1="187" y1="218" x2="282" y2="168"/>
    <line x1="322" y1="113" x2="562" y2="98"/>
    <line x1="562" y1="98"  x2="522" y2="183"/>
    <line x1="282" y1="168" x2="447" y2="193"/>
  </g>
  <g class="mesh-nodes">
    <!-- Cluster A — upper-left main camp (tight, 3 phones) -->
    <use href="#phone" x="60"  y="40"  width="24" height="36"/>
    <use href="#phone" x="95"  y="75"  width="24" height="36"/>
    <use href="#phone" x="130" y="42"  width="24" height="36"/>
    <!-- Cluster B — center stage area (slight spread, 3 phones) -->
    <use href="#phone" x="235" y="110" width="24" height="36"/>
    <use href="#phone" x="270" y="150" width="24" height="36"/>
    <use href="#phone" x="310" y="95"  width="24" height="36"/>
    <!-- Cluster C — back camp lower-right (tight, 3 phones) -->
    <use href="#phone" x="435" y="175" width="24" height="36"/>
    <use href="#phone" x="475" y="205" width="24" height="36"/>
    <use href="#phone" x="510" y="165" width="24" height="36"/>
    <!-- 3 outliers spread across the camp -->
    <use href="#phone" x="175" y="200" width="24" height="36"/>
    <use href="#phone" x="390" y="40"  width="24" height="36"/>
    <use href="#phone" x="540" y="80"  width="24" height="36"/>
  </g>
  <circle class="mesh-msg" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
</svg>
<p class="mesh-caption">Each phone hops messages to the next — no cell tower needed.</p>
</div>

---

## Get Started in 3 Steps

<div class="grid cards" markdown>

-   :material-cart:{ .lg } **1. Get a radio**

    ---

    The easiest path is the **RAK WisMesh Tag** (~$30) or **LILYGO T-Echo** (~$60). See our full picks.

    [Recommended Hardware](docs/recommended-hardware.md){ .md-button }

-   :material-cog:{ .lg } **2. Configure it for the Forest**

    ---

    There are a few specific settings you need to use to be compatible with the EF mesh. Don't get creative — just follow the steps.

    [How to Connect](docs/how-to-connect.md){ .md-button }

-   :material-account-group:{ .lg } **3. Find your squad**

    ---

    Scan the official EF channels QR, then set up your private squad channel. Then start texting.

</div>

---

## Need Help?

The EF Meshtastic crew lives in the official Electric Forest Discord, in the dedicated Meshtastic thread. Setup questions, troubleshooting, "is my node working?" — drop in.

<span style="display: flex; justify-content: center; margin: 1.5rem 0;">
    [:fontawesome-brands-discord: Ask in the EF Discord Meshtastic Thread](https://discord.com/channels/260909643574935553/1111482301730271232){ .md-button .md-button--primary target="_blank"}
</span>

*Not in the Discord? Join at [discord.gg/electricforest](https://discord.gg/electricforest){ target=_blank } first.*{ .discord-helper }

---

## Why Bring Meshtastic to the Forest?

Bebop'n around the Forest solo (and a little lost) is part of the magic. But there are moments where you actually need to find your squad — and cell service in Sherwood is famously spotty.

We had real success bringing these little radios to Forest last year. Setup is easier than it looks. And once you have one, you have it for every festival, backpacking trip, and emergency for years.

These devices **mesh** — every additional radio in the Forest makes the whole network stronger for everyone. Bring one. Bring two. Get your squad on.

---

<div class="ef-disclaimer" markdown>
**Heads up — this is unofficial.** This site is run by Forest fam, not by Electric Forest, Insomniac, or Madison House Presents. It's just a friendly guide to help you and your squad stay connected on-grounds. Everything here is community knowledge, shared in good faith.
</div>
