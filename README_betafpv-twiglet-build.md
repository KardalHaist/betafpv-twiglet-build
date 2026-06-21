# $57.93 Micro FPV Toothpick — Cheaper Than the MEPS King 59

Built a sub-$58 micro FPV drone from scratch using AliExpress welcome deals. Undercut the [MEPS King 59]() — a drone marketed as a budget build — by $1.07 on the drone itself, with a different flight controller, a 3D printed canopy, and printed battery mounts.

> Video demo: [(https://youtube.com/shorts/hndg69Q7bj8?feature=share)]()
> MEPS King 59 reference doc: [link TBD]()

Price comparison is drone-only (no TX or RX included in either number).

---

## Build Spec

| Component | Part | Notes |
|---|---|---|
| Frame | BETAFPV Twiglet Mini 2" | 85mm True-X, 26x26mm stack mount |
| FC / AIO | T-Motor F4 SX1280 AIO | STM32F411, SPI ELRS 2.4GHz, 6A ESC, integrated VTX |
| Motors | 1103 15000KV | AliExpress, 1S-2S |
| Camera | CADDX Ant Nano | 14x14mm |
| Radio | RadioMaster T8L | Screenless, integrated ELRS 2.4GHz, Mode 2 |
| Goggles | Generic 5.8GHz | 3" IPS, bands A/B/E/F/R |
| Battery | Lava 1S | |
| Canopy | AngryDonFPV — [Thing:4592267](https://www.thingiverse.com/thing:4592267) | 40° tilt, fin version, TPU 95A — printed |
| Battery mounts | Custom | Printed |

Betaflight 4.4.3, DSHOT300, CRSF protocol.

---

## Cost Breakdown

> **Total: $57.93** (drone only, excludes TX and goggles)

Used AliExpress new-account welcome deals — one deal per account. Not a scalable strategy, but it worked for this build.

Full receipt documentation: [docs/receipts.md]() — TBD

---

## What's in This Repo (eventually)

- [ ] Full receipt / BOM with actual paid prices
- [ ] Betaflight config dump
- [ ] Build photos
- [ ] STL files for battery mounts (canopy is from Thingiverse — link above)
- [ ] Wiring diagram
- [ ] Flight video

---

## Repo Structure

```
/
├── README.md
├── docs/
│   ├── bom.md              # full BOM with sourcing
│   ├── betaflight-config.md
│   ├── build-notes.md
│   └── receipts.md
├── media/
│   ├── photos/
│   └── video/
└── cad/
    └── battery-mounts/     # STL files
```

---


---

*Florida Tech — EE Freshman project
