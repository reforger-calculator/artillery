# 🎯 Spearhead Artillery Calculator

[![GitHub Pages](https://img.shields.io/badge/demo-live-brightgreen)](https://reforger-calculator.github.io/artillery/)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](#license)
[![Made for Arma Reforger](https://img.shields.io/badge/Arma%20Reforger-Spearhead%20Mod-orange)](https://reforger-calculator.github.io/artillery/)

A free, browser-based **artillery and mortar ballistic calculator** built for the **Spearhead mod** for **Arma Reforger**. Enter your position, a target grid, and current wind, and get an instant firing solution — azimuth, elevation, time of flight, peak altitude, and impact angle — corrected for wind drift.

**🔗 Live tool: [reforger-calculator.github.io/artillery](https://reforger-calculator.github.io/artillery/)**

---

## Features

- **Multiple weapon systems** with real ballistic tables:
  - M177 Howitzer
  - M821 Mortar (US)
  - O-832DU Mortar (RUS)
  - 2B9 Vasilek automatic mortar
  - AGS-17 automatic grenade launcher
  - BM-21 Grad multiple rocket launcher (9M22 OF, 3M16 Cluster, 9M28K Cluster)
- **Grid coordinate parsing** — supports 3-digit map grid, 4+ digit precise grid, and numpad sub-grid fine-tuning
- **Wind correction** — factors in wind direction and velocity for both range and azimuth drift
- **Mission history** — track multiple targets at once, edit coordinates inline, recalculates live when you switch weapons or ammo
- **No install, no accounts, no ads** — a static page that runs entirely in your browser

## Supported Coordinate Formats

| Format | Example | Use case |
|---|---|---|
| XY Grid (3-digit) | `050 080` | Read directly off the in-game map |
| XY Direct (4+ digit) | `05000 08000` | GPS or SAL drone laser readout |
| Elevation | `050 080 120` | Cursor position or GPS altitude |
| Numpad fine-tune | `050 080 120 94` | Subdivide the grid square using the numpad |

## Tech Stack

Plain HTML, CSS, and vanilla JavaScript — no build step, no dependencies. Ballistic data is stored as JSON tables and loaded dynamically per weapon.

## Contributing

Found a ballistic table with an error, or have data for a weapon that isn't listed yet? Screenshots of in-game ballistic reference cards are the easiest way to contribute — open an issue or a pull request.

## Disclaimer

This is a fan-made, community tool for the Spearhead mod for Arma Reforger. It is not affiliated with or endorsed by Bohemia Interactive.

## License

MIT
