---
hide:
  - navigation
title: Recommended Hardware
---

# :material-radio-handheld: Recommended Hardware for the Forest

You only need one radio to start. There are a lot of options out there — and a **lot of knock-offs**, especially fake antennas on Amazon. Buy from a trusted source.

!!! tip "What to actually buy"
    **For most people, get the WisMesh Tag (~$30)** — clips to your pack, works out of the box, just charge it and go.

    **If you want a screen on the device itself**, get the **LILYGO T-Echo (~$60)** — readable in direct sun (e-ink), longer range thanks to an external antenna.

    Either of these is a great Forest radio. Order one this week and you're set.

---

## :material-cellphone: Handheld Radios (carry these on you)

### LILYGO T-Echo (~$60)

A community favorite. E-ink screen (like a Kindle) so it's readable in direct Michigan sun and barely sips battery. External antenna means longer range than the card-style trackers.

|  |  |
|:--|:--|
| **Pros** | Screen to read messages without your phone &middot; More range than card-style nodes due to external antenna &middot; Ready out of the box &middot; Bluetooth + GPS &middot; Antenna can be upgraded for more range |
| **Cons** | A bit chunky &middot; The reset button is easy to press accidentally (Etsy has cases that cover it) |
| **Where to buy** | [Rokland (US, fast shipping)](https://store.rokland.com/products/lilygo-ttgo-meshtastic-t-echo-white-lora-sx1262-wireless-module-915mhz-nrf52840-gps-for-arduino){ target=_blank } &middot; [AliExpress (LILYGO official, ships from China)](https://www.aliexpress.com/item/1005003026107533.html){ target=_blank } |
| **Antenna upgrade** | [Muzi 17cm Whip](https://muzi.works/products/whip-antenna-17cm){ target=_blank } — biggest range boost for $12 |

---

### RAK WisMesh Tag (~$30)

Cheapest option that works out of the box. About the size of a credit card, clips to your pack. No screen — you check messages on your phone.

|  |  |
|:--|:--|
| **Pros** | Cheap &middot; Compact, clips to a backpack &middot; Ready to go &middot; Bluetooth + GPS &middot; Better battery than the T-1000e &middot; IP66 waterproof |
| **Cons** | No external antenna, so shorter range than the T-Echo &middot; Recharges via a magnetic pin cable (proprietary) &middot; No screen means you can't easily tell if it's online without checking your phone |
| **Where to buy** | [RAKwireless](https://store.rakwireless.com/products/wismesh-tag-meshtastic-gps-lora-tracker-ip66){ target=_blank } &middot; [Amazon](https://www.amazon.com/RAKwireless-MOKOSmart-Meshtastic-Compatible-Waterproof/dp/B0FYHPTPZD){ target=_blank } |

---

### Sensecap T-1000e (~$30-35)

Similar form factor to the WisMesh Tag. Most of us prefer the WisMesh Tag — better battery and a touch more range — but the T-1000e is widely available on Amazon for last-minute pickups.

!!! info "Make sure you buy the T-1000-E"
    There are several T-1000 trackers out there. Get the **T-1000-E** specifically — the others won't work for Meshtastic.

|  |  |
|:--|:--|
| **Pros** | Cheap &middot; Compact, clips to a pack &middot; Ready to go &middot; Bluetooth + GPS &middot; Available on Amazon for last-minute buys |
| **Cons** | No external antenna &middot; Proprietary magnetic charging &middot; No screen |
| **Where to buy** | [Seeed Studio (official)](https://www.seeedstudio.com/SenseCAP-Card-Tracker-T1000-E-for-Meshtastic-p-5913.html){ target=_blank } &middot; [Amazon](https://www.amazon.com/SenseCAP-Card-Tracker-T1000-Meshtastic/dp/B0DJ6KGXKB){ target=_blank } |

---

### LILYGO T-Deck (~$80)

Want to leave your phone in your tent? The T-Deck has a full physical keyboard and runs standalone. Niche but cool.

|  |  |
|:--|:--|
| **Pros** | Cheap for what it is &middot; Physical keyboard &middot; Bluetooth + GPS + Wifi &middot; Available on Amazon |
| **Cons** | Needs a big battery &middot; No external antenna &middot; Map setup is fiddly (you have to upload your own map files) — if GPS-on-the-device matters to you, skip this |
| **Where to buy** | [Rokland](https://store.rokland.com/products/lilygo-t-deck-portable-microcontroller-programmer-lora-915-mhz-h642){ target=_blank } &middot; [Amazon](https://www.amazon.com/LILYGO-ESP32-S3-LORA-89-2-8-inch-Development/dp/B0FBGX1VP5){ target=_blank } |

---

## :material-tower-fire: Want to Help the Mesh? Build a Camp Node.

Higher antenna = more range for everyone. If you've got camp infrastructure (a flag pole, a totem, a tall structure), you can host a node up high and dramatically extend the mesh for the whole community.

[See the Camp Nodes guide :material-arrow-right-bold:](camp-nodes.md){ .md-button .md-button--primary }

---

## :material-antenna: Antenna Upgrades

**This is the single best ~$12 you can spend on Meshtastic.** Stock antennas on most handhelds are mediocre. Swap to a real 915 MHz whip antenna and your range jumps significantly.

**Recommended antennas:**

- [Muzi 17cm Whip Antenna](https://muzi.works/products/whip-antenna-17cm){ target=_blank } — community favorite, SMA male, ~$12
- [ALFA 915 MHz 5dBi N-Type Outdoor 7"](https://atlavox.com/products/antenna-for-meshtastic-915mhz-n-type-outdoor-7-5dbi-alfa-aoa-915-5acm){ target=_blank } — for camp base stations
- [Rokland 5.8 dBi N-Male Omni Outdoor](https://store.rokland.com/collections/802-11ah-wi-fi-halow/products/5-8-dbi-n-male-omni-outdoor-915-mhz-antenna-large-profile-32-height-for-helium-rak-miner-2-nebra-indoor-bobcat){ target=_blank } — large outdoor, for permanent mounts

!!! warning "Watch out for fakes"
    The Meshtastic / LoRa antenna world is full of garbage knock-offs on Amazon. Buy from the trusted sources above, or directly from the antenna manufacturer.

**Tips:**

- For base station nodes, use a quality SMA or N-type cable — and **keep it short**. Every foot of cable adds some signal loss.
- "More dB" doesn't always mean "more coverage." A directional high-dB antenna in the wrong orientation can have *less* useful coverage than a modest omni.

---

## Need Help Picking?

Drop a message in the EF Discord Meshtastic thread — we're happy to talk through what fits your setup and budget.

<span style="display: flex; justify-content: center; margin: 1.5rem 0;">
    [:fontawesome-brands-discord: Ask the EF Discord](https://discord.com/channels/260909643574935553/1111482301730271232){ .md-button .md-button--primary target="_blank"}
</span>
