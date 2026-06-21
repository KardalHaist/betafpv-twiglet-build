$57.93 Micro FPV Toothpick — Cheaper Than the MEPS King 59

Built a sub-$58 micro FPV drone from scratch using AliExpress welcome deals. Undercut the MEPS King 59 — a drone marketed as a budget build — by $1.07 on the drone itself, with a different flight controller, a 3D printed canopy, and printed battery mounts.


Video demo: link TBD
MEPS King 59 reference doc: link TBD



Price comparison is drone-only (no TX or RX included in either number).


Build Spec

ComponentPartNotesFrameBETAFPV Twiglet Mini 2"85mm True-X, 26x26mm stack mountFC / AIOT-Motor F4 SX1280 AIOSTM32F411, SPI ELRS 2.4GHz, 6A ESC, integrated VTXMotors1103 15000KVAliExpress, 1S-2SCameraCADDX Ant Nano14x14mmRadioRadioMaster T8LScreenless, integrated ELRS 2.4GHz, Mode 2GogglesGeneric 5.8GHz3" IPS, bands A/B/E/F/RBatteryLava 1SCanopyAngryDonFPV — Thing:459226740° tilt, fin version, TPU 95A — printedBattery mountsCustomPrinted

Betaflight 4.4.3, DSHOT300, CRSF protocol.


Cost Breakdown


Total: $57.93 (drone only, excludes TX and goggles)



Used AliExpress new-account welcome deals — one deal per account. Not a scalable strategy, but it worked for this build.

Full receipt documentation: docs/receipts.md — TBD


What's in This Repo (eventually)


 Full receipt / BOM with actual paid prices
 Betaflight config dump
 Build photos
 STL files for battery mounts (canopy is from Thingiverse — link above)
 Wiring diagram
 Flight video



Repo Structure

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


Notes / Known Issues


Current sensor reads garbage — ibata_scale calibration is wrong, capacity drawn numbers are not accurate
1103 motors take 1.5mm shaft props — do not use 1218 props (wrong shaft size), need 2035 or 2040
VTX set to Raceband R Ch1 at 25mW



Florida Tech — EE Freshman project, Spring 2026
