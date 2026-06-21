[build-notes.md](https://github.com/user-attachments/files/29180639/build-notes.md)[Upload# Build Notes

## Component Spec

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

## Issues Encountered

**Wrong props shipped / ordered**

1103 motors have a 1.5mm shaft. Tried fitting 1218 props — those are designed for tiny whoop builds with 1.0mm shafts. They don't seat. Correct props for this build are 2035 or 2040 with a 1.5mm bore.

**ELRS version mismatch**

FC shipped with Betaflight 4.3.1. After flashing to 4.4.3, ELRS firmware on the SX1280 chip was mismatched with the TX module firmware. Had to update ELRS on both ends to the same version before the link would establish.

**Current sensor calibration**

The `ibata_scale` value was set for a 10mΩ shunt but the board uses 100mΩ. This caused the capacity drawn reading to be wildly wrong (showing 2000+ mAh on a 1S cell). Do not trust capacity drawn numbers until this is corrected in CLI:
```
set ibata_scale = XX
save
```
Correct value TBD — needs bench measurement against a known current source.

**Motor bearing damage**

Two right-side motors showed bearing damage on inspection. Likely from a prior crash or shipping. Replaced all four motors with the 1103 15000KV units listed above.

**First flight cutout**

Battery was at 3.56V resting before first flight attempt. Under motor load it sagged below FC brownout threshold and cut power immediately. Always check resting voltage before arming — 1S should be at 4.0V+ before flight.

---

## What's Still Unresolved

- `ibata_scale` calibration — current sensor reads wrong
- Props — need 2035 or 2040, not yet ordered
ing build-notes.md…]()

