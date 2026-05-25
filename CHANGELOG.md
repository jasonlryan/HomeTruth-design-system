---
title: Design System Changelog
type: changelog
updated: 2026-05-25
---

# Changelog

All notable changes to the HomeTruth Design System are recorded here.
The format follows [Keep a Changelog](https://keepachangelog.com/); the
system uses [semantic versioning](https://semver.org/).

## [0.1.0] — 2026-05-25

### Added

- Initial design-system folder structure and `design-system.md` index.
- Foundations populated from the HomeTruth Development Style Guide (14.08.2025)
  and `BRAND.md`: colour, typography, spacing & layout, gradients.
- Design tokens: `tokens/tokens.json` (W3C DTCG format) and `tokens/tokens.css`
  (CSS custom properties).
- Logos folder with the full logo (light/dark) and brand mark, plus usage rules.
- Icons folder with the building-block mark and naming/sizing conventions.
- Scaffolded `components/`, `imagery/` and `voice-and-tone/` folders.

### Changed

- Typography tokens now prefer the self-hosted `HomeTruth Gill Sans` webfont
  family before falling back to local Gill Sans/system fonts.

### Added

- Home lifecycle building-block SVG motifs for Purchase, Maintain, Improve and
  Sell.
- Brand provenance foundation documenting the source hierarchy for colour
  decisions, the current accepted UI values and how to treat conflicting logo
  artwork/style-guide swatches.

### Changed

- Colour, logo and token docs now state that UI colour decisions are
  provenance-based: `BRAND.md` plus the product token bridge are canonical for
  UI, while approved artwork files remain canonical for logo artwork.
