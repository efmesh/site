---
hide:
  - navigation
title: Camp Nodes
---

# :material-tower-fire: Setting Up a Camp Node

Want to go big? A high-up node at your camp helps everyone — especially folks with smaller, less-powerful handhelds. **Height is might.** The higher you can mount your antenna, the more of the Forest gets reliable mesh coverage.

!!! warning "Stick to Client role unless you've been told otherwise"
    Even if your node is up high and powered all weekend, **do not set it to Repeater or Router** unless someone in the [EF Discord](https://discord.com/channels/260909643574935553/1111482301730271232){ target=_blank } has explicitly given you the OK. Misconfigured Router/Repeater nodes break the mesh for the entire Forest. Default `Client` mode still helps a ton at elevation.

---

## Pre-Built Options (Easy Mode)

Want to plug-and-play? Here are pre-built nodes that work well as camp infrastructure. No soldering, no firmware drama.

### SenseCAP Solar Node P1 Pro

Self-contained solar node. Plant it, point the panel at the sky, walk away for the weekend.

|  |  |
|:--|:--|
| **Pros** | Built-in solar panel + battery &middot; Built-in GPS &middot; Panel adjustable independently from antenna &middot; Reasonably priced |
| **Cons** | No wifi |
| **Where to buy** | [Seeed Studio (official)](https://www.seeedstudio.com/SenseCAP-Solar-Node-P1-Pro-for-Meshtastic-LoRa-p-6412.html){ target=_blank } |

---

### WisMesh Repeater Mini

Discreet enough to stash on top of a tall structure without drawing attention. Lots of mounting options including magnets.

|  |  |
|:--|:--|
| **Pros** | Looks unassuming (good for unsupervised mounts) &middot; Tons of mounting options including magnets &middot; Built-in solar + battery &middot; Built-in GPS &middot; Cheap |
| **Cons** | No wifi &middot; Solar panel not adjustable |
| **Where to buy** | [RAKwireless](https://store.rakwireless.com/products/wismesh-meshtastic-solar-repeater-mini){ target=_blank } |

---

### Atlavox Beacon (Pre-Configured)

If money is no object and you want something insanely rugged — strap it to a flag pole, a truck roof, a tree. This thing is a tank.

|  |  |
|:--|:--|
| **Pros** | Built-in solar + battery &middot; Built-in GPS &middot; Panel adjustable independently from antenna &middot; Best-of-the-best components pre-selected |
| **Cons** | Expensive &middot; No wifi |
| **Where to buy** | [Atlavox (pre-configured "Outpost" config)](https://atlavox.com/products/atlavox-beacon-solar-meshtastic-node-outpost-config){ target=_blank } &middot; [Customizable version](https://atlavox.com/products/atlavox-beacon-solar-meshtastic-node){ target=_blank } |

---

### Heltec V4 Pre-Built (Etsy)

Want wifi so you can connect via a hotspot? This is probably the best pre-built option with wifi support. Needs constant power, so only good if you've got a reliable hookup at camp.

|  |  |
|:--|:--|
| **Pros** | Wifi &middot; Configure and go |
| **Cons** | Expensive &middot; No built-in GPS (you have to manually set coordinates) &middot; Requires constant power (no solar) |
| **Where to buy** | [Etsy listing](https://www.etsy.com/listing/1877304075/meshcoremeshtastic-outdoor-repeater?ref=user_profile){ target=_blank } |

---

### Harbor Freight Solar Light Hack

Comfortable with a screwdriver and some cable connections? Convert a $30 Harbor Freight solar light into a fully solar Meshtastic node. Great DIY project.

|  |  |
|:--|:--|
| **Pros** | Built-in solar + battery &middot; Dirt cheap |
| **Cons** | No built-in GPS (manual coordinate entry) |
| **How to build** | [Official Meshtastic guide](https://meshtastic.org/docs/community/enclosures/rak/harbor-breeze-solar-hack/){ target=_blank } &middot; [Ben Jordan's YouTube video](https://youtu.be/W_F4rEaRduk?t=180){ target=_blank } |

---

## Antennas Matter More Than the Node

For camp nodes, your antenna is **more important than the radio itself**. A $400 radio with a stock antenna will be outperformed by a $100 radio with a good external antenna mounted high.

**Top picks for camp base stations:**

- [Muzi 17cm Whip](https://muzi.works/products/whip-antenna-17cm){ target=_blank } — ~$12, great upgrade over any handheld stock antenna
- [ALFA 915 MHz 5dBi N-Type Outdoor](https://atlavox.com/products/antenna-for-meshtastic-915mhz-n-type-outdoor-7-5dbi-alfa-aoa-915-5acm){ target=_blank } — built for outdoor permanent mounts
- [Rokland 5.8 dBi N-Male Omni Outdoor](https://store.rokland.com/collections/802-11ah-wi-fi-halow/products/5-8-dbi-n-male-omni-outdoor-915-mhz-antenna-large-profile-32-height-for-helium-rak-miner-2-nebra-indoor-bobcat){ target=_blank } — for permanent rooftop or pole mounts

**Cable tips:**

- Use quality SMA or N-type cable
- **Keep the cable short.** Every foot adds signal loss.
- For long runs, you'll want LMR-400 or better

---

## The Observatory Stage Letter

The EF Meshtastic community has drafted an open letter to Electric Forest staff requesting permission to host a single, high-elevation Meshtastic node at the **Observatory Stage** — a backbone repeater that would give the entire grounds line-of-sight coverage.

It's a community-led ask, not endorsed by EF.

[:material-pine-tree: Read the letter](wish-machine-request.md){ .md-button }

---

## More Advanced Options?

If you want to roll your own — pick your own boards, antennas, batteries, cases — check the [Advanced Options](advanced.md) page.

---

## Need Help Picking a Camp Node?

<span style="display: flex; justify-content: center; margin: 1.5rem 0;">
    [:fontawesome-brands-discord: Ask in the EF Discord](https://discord.com/channels/260909643574935553/1111482301730271232){ .md-button .md-button--primary target="_blank"}
</span>
