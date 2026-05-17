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

[Meshtastic](https://meshtastic.org){ target=_blank } is a tiny radio that clips to your pack and lets you text your friends across the Forest **even when cell service is dead**. No subscription. No SIM card. No monthly fee. About $30 to get on the mesh.

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
        <span class="ef-carrier">Meshtastic</span>
        <span class="ef-battery" aria-hidden="true">
          <svg viewBox="0 0 22 10" width="22" height="10"><rect x="0.5" y="0.5" width="18" height="9" rx="2" fill="none" stroke="#bda7f5" stroke-width="1"/><rect x="2" y="2" width="13" height="6" rx="1" fill="#b6f0a8"/><rect x="19.5" y="3" width="2" height="4" rx="0.5" fill="#bda7f5"/></svg>
        </span>
      </div>
      <div class="ef-chatheader">
        <span class="ef-meshicon" aria-hidden="true">
          <svg viewBox="0 0 24 24" width="16" height="16" fill="none" stroke="#b6f0a8" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"><circle cx="5" cy="6" r="2"/><circle cx="19" cy="6" r="2"/><circle cx="12" cy="18" r="2"/><line x1="5" y1="6" x2="19" y2="6"/><line x1="5" y1="6" x2="12" y2="18"/><line x1="19" y1="6" x2="12" y2="18"/></svg>
        </span>
        <span class="ef-chattitle">Squad Chat</span>
      </div>
      <div class="ef-chatbody">
        <div class="ef-chat-track">
        <div class="ef-msg ef-msg--in ef-msg--1"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">happy forest &#127795; made it through the gate!</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--2"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">in line at trading post, brb</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--3"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">set up at camp K3, look for the orange flag</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--4"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">happy forest fam! 30min out from gate</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--5"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">sherwood opens at sundown, we heading in?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--6"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">battery dying, finding power &#128267;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--7"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">vibe check &#10024; everyone good?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--8"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">all good! kandi for days &#127752;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--9"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">this set at ranch arena is INSANE &#128293;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--10"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">anyone heading to sherwood?</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--11"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">i&rsquo;m at carousel club, under the hands of love &#127904;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--12"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">drop a pin, can&rsquo;t find anyone</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--13"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">happy forest! coffee at lucky lake?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--14"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">wook squad assembling at camp</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--15"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">PLURR vibes &#9996;&#128156;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--16"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">yoga at the meadow in 20</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--17"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">headliner at 9pm, rally at 8?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--18"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">trading kandi at the totem &#127752;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--19"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">giving tree at midnight, who&rsquo;s in</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--20"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">im at the observatory &#128301;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--21"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">this DJ is unreal, you need to be here</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--22"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">lost my flow toys deep in sherwood &#128557;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--23"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">found a sherwood shepherd, all good</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--24"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">rain incoming &#9748; head back?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--25"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">happy forest day 3!! &#9728;&#65039;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--26"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">battery at 3%, save my pin</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--27"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">trading post run for sunscreen</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--28"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">anyone got pashminas to trade?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--29"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">sherwood was MAGIC last night</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--30"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">lineup tonight is stacked</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--31"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">rally at ranch arena 7pm</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--32"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">see y&rsquo;all there &#128156;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--33"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">saturday hits different, fam &#127795;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--34"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">happy forest fam &#10084;&#65039;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--35"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">caught sunrise from the dunes, unreal</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--36"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">back to camp for a nap, regroup at 6?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--37"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">drop a pin if you&rsquo;re napping, i&rsquo;ll find you</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--38"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">sunset at the observatory deck?</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--39"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">yes! bring the totem</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--40"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">on my way, totem squad assemble &#128156;&#127795;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--41"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">just rolled in! where&rsquo;s camp?</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--42"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">row K, third in, orange flag still up</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--43"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">anyone near the hangar? lost my crew</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--44"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">heading that way in 10, hold tight</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--45"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">CARLLLLL &#128514;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--46"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">CARRRRL has been spotted at tripolee</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--47"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">water refill run, anyone need bottles topped</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--48"><div class="ef-msg__inner"><span class="ef-name">kai</span><span class="ef-bubble">YES bring mine pls, im at the chapel</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--49"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">this b2b is melting me &#128525;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--50"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">which stage?? coming</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--51"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">jubilee, back left by the trees</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--52"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">mesh saved us again, no bars anywhere</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--53"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">surprise guest at ranch arena rn, RUN</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--54"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">on the way! leaving sherwood now</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--55"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">found a charging tent by main street &#128268;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--56"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">dropping a pin at the observatory deck</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--57"><div class="ef-msg__inner"><span class="ef-name">kai</span><span class="ef-bubble">food truck line on main street is wild rn</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--58"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">grilled cheese cart by general store, no line</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--59"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">bless you, on my way &#128591;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--60"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">just hugged 3 strangers, forest is healing</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--61"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">totem squad assemble at giving tree 11pm</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--62"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">bringing the disco ball totem &#128131;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--63"><div class="ef-msg__inner"><span class="ef-name">riley</span><span class="ef-bubble">first forest! where&rsquo;s the trash bar??</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--64"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">deep in sherwood, follow the disco lights</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--65"><div class="ef-msg__inner"><span class="ef-name">riley</span><span class="ef-bubble">found it!!! omg this place &#129327;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--66"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">welcome to forest, riley &#127795;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--67"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">weather hold? sky looks sus &#9928;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--68"><div class="ef-msg__inner"><span class="ef-name">kai</span><span class="ef-bubble">radar shows it passing in 20, hold at camp</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--69"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">mud at ranch lol boots up</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--70"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">forest weather has range</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--71"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">camp shower line moving fast btw</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--72"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">ranch arena set is going OFF rn</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--73"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">lost a wristband, anyone seen one near hangar?</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--74"><div class="ef-msg__inner"><span class="ef-name">riley</span><span class="ef-bubble">turned in one at info, check there!</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--75"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">on my way to grab it, thx riley</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--76"><div class="ef-msg__inner"><span class="ef-name">kai</span><span class="ef-bubble">grand artique has a secret set in 30</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--77"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">SAY LESS, rallying the crew</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--78"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">sunrise at the meadow tmrw, who&rsquo;s in</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--79"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">IN. setting alarms now</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--80"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">forest family forever &#128156;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--81"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">neighbor camp brought us pancakes &#129374;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--82"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">trade you stickers for sunscreen?</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--83"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">come thru, K3 has spf for days</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--84"><div class="ef-msg__inner"><span class="ef-name">theo</span><span class="ef-bubble">finally synced to mesh, hi forest fam</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--85"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">welcome theo! we&rsquo;re at carousel club</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--86"><div class="ef-msg__inner"><span class="ef-name">riley</span><span class="ef-bubble">this is way better than cell, im a convert</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--87"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">told u! mesh gang for life</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--88"><div class="ef-msg__inner"><span class="ef-name">sam</span><span class="ef-bubble">that set was UNREAL, no words</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--89"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">carousel selfie incoming, get in here</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--90"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">running, 2 min out</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--91"><div class="ef-msg__inner"><span class="ef-name">kai</span><span class="ef-bubble">sunday already?? noooo &#128557;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--92"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">make it count, see u in sherwood at sundown</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--93"><div class="ef-msg__inner"><span class="ef-name">finn</span><span class="ef-bubble">last sherwood run, who&rsquo;s coming &#127904;</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--94"><div class="ef-msg__inner"><span class="ef-name">alex</span><span class="ef-bubble">all of us. all of us.</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--95"><div class="ef-msg__inner"><span class="ef-name">riley</span><span class="ef-bubble">cried twice today and im not even sorry</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--96"><div class="ef-msg__inner"><span class="ef-name">theo</span><span class="ef-bubble">love yall. see you next forest &#128156;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--97"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">drop pins one last time before we scatter</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--98"><div class="ef-msg__inner"><span class="ef-name">jess</span><span class="ef-bubble">pinned. giving tree. one more group hug</span></div></div>
        <div class="ef-msg ef-msg--in ef-msg--99"><div class="ef-msg__inner"><span class="ef-name">mira</span><span class="ef-bubble">happy forest fam. till the trees light up again &#127795;&#128156;</span></div></div>
        <div class="ef-msg ef-msg--out ef-msg--100"><div class="ef-msg__inner"><span class="ef-name">you</span><span class="ef-bubble">see you in the forest &#10024;</span></div></div>
        </div>
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
  <circle class="mesh-msg mesh-msg--1" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
  <circle class="mesh-msg mesh-msg--2" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
  <circle class="mesh-msg mesh-msg--3" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
  <circle class="mesh-msg mesh-msg--4" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
  <circle class="mesh-msg mesh-msg--5" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
  <circle class="mesh-msg mesh-msg--6" r="5" fill="#ffb84d" stroke="#fff" stroke-width="1.5"/>
</svg>
<p class="mesh-caption">Packets hop phone to phone in parallel — no cell tower needed.</p>
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
