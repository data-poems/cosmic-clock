# Cosmic Clock 2026

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://dr.eamer.dev/datavis/poems/cosmic-clock/)

A hypnotic visualization of time at every scale. Watch the year unfold through concentric rings that track everything from seconds to months, with lunar phases, zodiac constellations, and the major events of 2026 marked along the way.

**[View Live Demo →](https://dr.eamer.dev/datavis/poems/cosmic-clock/)**

## What It Does

13 concentric rings, each representing a different scale of time, all synchronized to the current moment:

- **Time rings**: Minutes, hours (progress arcs)
- **Calendar rings**: Weekday, day of month, month, ISO week number
- **Celestial rings**: Lunar phases (8-phase cycle), zodiac constellations with line art
- **Seasonal ring**: Four color-coded seasonal bands with active label
- **Events ring**: 40+ events for 2026 (holidays, sports, astronomical)
- **Meteor shower ring**: 11 major showers with activity arcs and peak markers (solar longitude timing from IAU)
- **Daylight ring**: Variable-width waveform showing hours of daylight (~40°N sinusoidal model)
- **Planets ring**: 5 naked-eye planets at real-time ecliptic longitude positions (JPL J2000 Keplerian elements)

The whole thing animates smoothly in real-time. Hover or tap any ring segment for contextual details.

## Themes

I built 24 visual themes because why not. Each has its own center pulse animation:

### Organic
- **Bioluminescent** – Multi-layered glow like deep-sea creatures
- **Aurora** – Northern lights shimmer

### Glassmorphism (3 variants)
- **Glass, Frost, Aurora** – Translucent frosted layers

### Skeuomorphic Metals (14 variants)
- **Brass, Chrome, Cockpit, Bronze, Copper, Titanium, Rose Gold**
- **Gunmetal, Platinum, Obsidian, Amber, Jade, Onyx**
- Metallic orbs with 3D highlights and beveled edges
- Cockpit theme includes retro CRT scanlines

### Swiss Design (3 variants)
- **Railway, Poster, Classic** – Clean geometric precision
- Inspired by International Typographic Style

### Neumorphism (3 variants)
- **Neu, Light, Dark** – Soft embossed gradients with subtle shadows

## 2026 Events

The outermost ring marks major events throughout the year:

- **Astronomical**: Eclipses, equinoxes, solstices, planetary alignments
- **Sports**: Winter Olympics (Milan-Cortina), FIFA World Cup, Super Bowl
- **Cultural**: Major international holidays across traditions
- **Scientific**: Spacecraft milestones, celestial phenomena

## Tech Stack

Pure vanilla JavaScript and Canvas 2D. No frameworks, no build tools, no dependencies. Just open `index.html` in a browser.

The rendering engine handles:
- Real-time animation via `requestAnimationFrame`
- Theme-aware color palettes and effects
- Responsive layout for mobile and desktop
- Interactive tooltips with touch and mouse support

## Running Locally

```bash
# Serve with any HTTP server
python3 -m http.server 8000

# Then open http://localhost:8000
```

(You can open `index.html` directly, but a local server avoids CORS issues.)

## Data Sources

- **Astronomical events**: NASA JPL Horizons, International Astronomical Union
- **Lunar phases**: Calculated from NASA/USNO 2026 new moon reference (Jan 29, 12:36 UTC)
- **Zodiac constellations**: Traditional constellation patterns with accurate star positions
- **Sports events**: Official Olympic Committee and FIFA schedules
- **Holidays**: International calendar data

## License

MIT License – use it however you want.

## Author

Built by [Luke Steuber](https://lukesteuber.com)

More projects at [dr.eamer.dev](https://dr.eamer.dev)
