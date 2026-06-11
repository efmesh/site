---
hide:
  - navigation
title: Advanced Options
---

# :material-tools: Advanced Options

For folks who want to roll their own hardware, push more power, or experiment with mesh-monitoring software. **Most people don't need this.** A WisMesh Tag or T-Echo and you're set for the Forest.

---

## High-Power Nodes

### B&Q Station G2

The most powerful consumer Meshtastic radio available. Most handhelds put out ~0.25–0.5 watts. The Station G2 puts out **1 watt**, so it reaches dramatically further. Fantastic base station / static node.

![B&Q Station G2 with a whip antenna attached, sitting upright on a desk](../assets/img/advanced/station-g2.jpg){ .ef-advanced-img }

|  |  |
|:--|:--|
| **Pros** | 1W transmit power (vs ~0.5W for most) &middot; Modular — can add GPS, etc. &middot; Wifi (accessible over your local network) &middot; Excellent for a base station |
| **Cons** | Sells out fast &middot; 2–3 week lead time &middot; Power-hungry, no built-in battery &middot; Known to "talk loud, be deaf" (great TX, weaker RX) &middot; Expensive |
| **What you need** | An antenna (upgrade from stock) |
| **Where to buy** | [B&Q Consulting (official)](https://shop.uniteng.com/product/meshtastic-mesh-device-station-edition/){ target=_blank } |
| **Guide** | [Uniteng wiki](https://wiki.uniteng.com/en/meshtastic/station-g2){ target=_blank } |

---

### Heltec V4

Newer and more available than the Station G2. Same 1W output. Open-source friendly.

![Heltec WiFi LoRa 32 V4 board with built-in OLED display and USB-C](../assets/img/advanced/heltec-v4.jpg){ .ef-advanced-img }

|  |  |
|:--|:--|
| **Pros** | Newer, easier to find than Station G2 &middot; 1W transmit power &middot; Modular — add GPS, accessories &middot; Wifi &middot; Great base station &middot; Some folks turn these into solar nodes (with effort) |
| **Cons** | Newer = some early bugs still &middot; Power-hungry, no built-in battery (you have to add one) |
| **What you need** | Antenna (upgrade from stock) &middot; A case &middot; Battery (if portable) |
| **Where to buy** | [Rokland](https://store.rokland.com/products/heltec-wifi-lora-32v4-esp32s3-sx1262-lora-node-meshtastic-lorawan){ target=_blank } &middot; [Etsy (cases & prebuilt)](https://www.etsy.com/search?q=heltec%20v4&ref=search_bar){ target=_blank } |

---

## DIY Build Kits

### RAK Wireless WisBlock Starter Kit

Most flexible DIY option. Pick your case, battery, antenna, modules. Super power-efficient — great base for solar nodes. **And it's the cheapest path to a 1W node** if you're willing to swap the radio module for a 1W booster (more on that below).

![RAK Wireless WisBlock Starter Kit — base board with RAK4631 core module unsocketed alongside](../assets/img/advanced/rak-wisblock-starter.jpg){ .ef-advanced-img }

|  |  |
|:--|:--|
| **Pros** | Cheaper than a pre-built &middot; Massively customizable &middot; Super power-efficient (great for solar) &middot; Can be built as a 1W node with a booster module |
| **Cons** | Requires time, patience, and some technical chops &middot; Need to source case, battery, antenna separately |
| **Buy the kit** | [RAK Wireless (international)](https://store.rakwireless.com/products/wisblock-meshtastic-starter-kit){ target=_blank } &middot; [Rokland (US distributor)](https://store.rokland.com/products/rak-wireless-wisblock-meshtastic-starter-kit){ target=_blank } |
| **Case options** | [Etsy — Sentinel case](https://www.etsy.com/listing/1705600327/sentinel-rak-wisblock-rak4631-meshtastic){ target=_blank } &middot; [Etsy — mini box](https://www.etsy.com/listing/1671316836/rak-wireless-wisblock-mini-box-for){ target=_blank } &middot; [3D printable](https://www.yeggi.com/q/rak+wisblock/){ target=_blank } |
| **Antenna guide** | [Meshtastic antenna docs](https://meshtastic.org/docs/hardware/antennas/){ target=_blank } |
| **Build guide** | [RAK WisBlock devices on Meshtastic docs](https://meshtastic.org/docs/hardware/devices/rak/){ target=_blank } |

#### Why add a 1W booster?

The default LoRa radio on most handhelds and starter kits transmits around **22 dBm (~160 mW)** — and in the US/AU 915 MHz band, regulation caps a stock node well under a watt. A 1W booster module pushes that to **30 dBm = 1000 mW**, roughly **6× the radiated power** of a stock node.

Because free-space range scales with the square root of power, **~6× the power gets you roughly 2–2.5× usable range** in the real world (more in clean line-of-sight, less through bodies and trees).

At the Forest specifically, this is the difference between **in-mesh and off-mesh** for venue-fringe campers — camp-to-stage hops can stretch 0.5–1.5 miles with bodies, RVs, and tree cover in the way. A 1W node + a decent whip + a few feet of elevation (totem, pole, roof of a van) is the high-leverage stack.

The KDHD Stuff scratch-build walkthrough is a great reference if you want to see a WisBlock + booster + solar repeater built end-to-end: [Scratch Build Repeater for Meshtastic and MeshCore](https://youtu.be/97d0KVdXgGQ){ target=_blank } (~50 min, parts list in the description).

If you don't want to assemble anything, **skip to the [WisMesh Station](#rak-wismesh-station-plug-and-play-1w) below** — same 1W output, plug-and-play.

---

### RAK WisMesh Station (plug-and-play 1W)

The plug-and-play 1W camp node — same power class as the WisBlock + booster build above, but assembled, configured, and ready to run out of the box. If "spend a Sunday soldering" sounds like a chore, this is the easy button.

|  |  |
|:--|:--|
| **Pros** | True 1W (30 dBm) on the HP variant &middot; Pre-installed meshtasticd, MQTT broker, Node-RED, Grafana &middot; Full metal enclosure &middot; Runs on a Raspberry Pi 4 — wifi + ethernet + USB built-in &middot; Includes LoRa antenna, GPS antenna, power adapter, 16GB SD card |
| **Cons** | More expensive than rolling your own (~$170+) &middot; AC powered (no built-in battery — wire it to a USB battery bank or AC at camp) &middot; Heavier than a handheld (~630g) |
| **Variants** | **WisMesh Station** (RAK8622) — 22 dBm / ~160 mW, ~$169.99 &middot; **WisMesh Station HP** (RAK8623) — 30 dBm / 1W, ~$175.99 (get this one if you want the range boost) |
| **What's in the box** | WisMesh Station unit &middot; LoRa antenna &middot; GPS antenna &middot; Power adapter &middot; 16GB SD card |
| **Where to buy** | [RAK Wireless store](https://store.rakwireless.com/products/meshtastic-gateway-raspberry-pi-wismesh-station){ target=_blank } |

**Why this is the easiest path to 1W coverage**: every other 1W option on this page either ships as a board you have to case + power + antenna yourself (Station G2, Heltec V4), or requires you to swap radio modules and source parts (WisBlock + booster). The WisMesh Station HP arrives assembled, in a metal enclosure, with antennas in the box and the software pre-flashed. Plug in USB-C, screw on the antenna, you're a 1W node.

---

## Software for Power Users

### MeshMonitor

A self-hosted web tool that auto-acknowledges messages and runs auto-traceroutes. Great for nerds running infrastructure nodes — typically deployed on a Raspberry Pi at camp. Helps the mesh self-heal by mapping connectivity automatically.

If you're comfortable with self-hosted tools and a Pi, [check out MeshMonitor](https://meshmonitor.org){ target=_blank }.

### MeshSense

Don't want to mess with a Pi? **MeshSense** runs on your laptop (Mac/PC/Linux) and does auto-traceroutes that help strengthen the mesh. Easier on-ramp than MeshMonitor.

[MeshSense by Affirmatech](https://affirmatech.com/meshsense){ target=_blank }

---

## Antennas (Deep Dive)

Recommended antennas:

- [Muzi 17cm Whip](https://muzi.works/products/whip-antenna-17cm){ target=_blank } — handheld upgrade, SMA male, ~$12
- [ALFA 915 MHz 5dBi N-Type 7" Outdoor](https://atlavox.com/products/antenna-for-meshtastic-915mhz-n-type-outdoor-7-5dbi-alfa-aoa-915-5acm){ target=_blank } — base station omni
- [Rokland 5.8 dBi N-Male Omni Outdoor (large)](https://store.rokland.com/collections/802-11ah-wi-fi-halow/products/5-8-dbi-n-male-omni-outdoor-915-mhz-antenna-large-profile-32-height-for-helium-rak-miner-2-nebra-indoor-bobcat){ target=_blank } — permanent outdoor mounts

Tips:

- **Watch out for fakes on Amazon** — antennas are the most counterfeited Meshtastic accessory. Buy from the trusted sources above.
- For base stations, use quality SMA or N-type cable. **Keep the cable short** — every foot adds signal loss.
- **More dB ≠ more coverage.** A directional high-dB antenna in the wrong orientation has less useful coverage than a modest omni.

![Antenna gain explanation — diagram showing how higher-dBi antennas flatten the radiation pattern, trading vertical reach for a longer but thinner horizontal beam](../assets/img/advanced/antenna-gain-pattern.png){ .ef-advanced-img }

---

## Example Setups

Folks in the community have shared their builds. Drop yours in the [EF Discord](https://discord.com/channels/260909643574935553/1514411058066882671){ target=_blank } (not in the Discord? join at [discord.gg/electricforest](https://discord.gg/electricforest){ target=_blank } first) and we'll feature it here.

### Cube Totem Mount

A T-Echo mounted to a [3D-printed bracket](https://makerworld.com/en/models/519487-lilygo-t-echo-bracket-with-1-4-tripod-mount#profileId-435876){ target=_blank } with a tripod-cheese-board adapter, riding on top of a Hyper Cube totem. Visible from across camp and high enough to push range significantly.

![Underside view of a Hyper Cube totem with a T-Echo mounted on a 3D-printed bracket and tripod adapter, antenna pointing up](../assets/img/advanced/cube-totem-mount.jpg){ .ef-advanced-img }

### G2 Mobile Setup

A Station G2 powered via USB-C, with an SMA cable running out to a roof-mounted antenna on a vehicle. Functions as a mobile base station that follows you to and from camp.

### Test Setup (T-Echo + 1W Base)

1× T-Echo handheld + 1× 1W base station (Station G2, Heltec V4, or a WisBlock with booster) = easily 1+ mile range hip-height. Dead spots at sharp elevation drops or through dense tree cover. Two-node minimum to start seeing real benefit.

![Tall fiberglass antenna pole erected in a backyard garden serving as the test base station](../assets/img/advanced/test-setup-pole.jpg){ .ef-advanced-img }

![Screenshot of the Meshtastic app showing a portable node mapped 0.955 miles away from base — clean signal through suburban terrain](../assets/img/advanced/test-setup-range-map.jpg){ .ef-advanced-img }

---

## Need Help?

<span style="display: flex; justify-content: center; margin: 1.5rem 0;">
    [:fontawesome-brands-discord: Ask in the EF Discord](https://discord.com/channels/260909643574935553/1514411058066882671){ .md-button .md-button--primary target="_blank"}
</span>

*Not in the Discord? Join at [discord.gg/electricforest](https://discord.gg/electricforest){ target=_blank } first.*{ .discord-helper }
