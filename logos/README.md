---
title: Logos
type: asset-library
category: logos
status: stable
updated: 2026-05-25
owner: Jason Ryan
tags:
  - design-system
  - brand
  - logo
assets:
  - hometruth-logo.png
  - hometruth-logo-dark.png
  - hometruth-icon.svg
---

# Logos

The HomeTruth logo is the foundation of the brand identity. It has two parts:
the **building-block mark** (the "TH" square in three colours) and the
**wordmark** ("Home" + "Truth" set in balanced Gill Sans weights, with "Truth"
in cyan).

## Files in this folder

| File | Format | Use |
|------|--------|-----|
| `hometruth-logo.png` | PNG | Full logo for light backgrounds |
| `hometruth-logo-dark.png` | PNG | Full logo for dark backgrounds |
| `hometruth-icon.svg` | SVG | Building-block mark only (scalable, app icon, favicon) |

## Logo anatomy

- **Mark:** the building-block "TH" square — orange, purple and cyan blocks.
  It represents the smart building blocks of the HomeTruth service.
- **Wordmark:** "HomeTruth" — "Home" in neutral, "Truth" in cyan.
- **Full logo:** mark + wordmark locked together, as used in the nav and hero.

## Artwork colours

The printed logo artwork uses slightly different hex values from the digital
UI palette. Both are correct in their context:

| Element | Logo artwork | UI token |
|---------|--------------|----------|
| Orange block | `#FD6815` | `#E8651A` (`--ht-orange`) |
| Purple block | `#7B4B9E` | `#8B3FA0` (`--ht-purple`) |
| Cyan block | `#19B0F0` | `#00B4D8` (`--ht-cyan`) |

Use the **logo artwork** SVG as-is for the mark. Use the **UI tokens** for
everything else (backgrounds, buttons, type). Do not recolour the logo to the
UI tokens.

## Usage rules

- **Clear space:** keep clear space around the logo equal to the height of one
  building block. Nothing should intrude into it.
- **Minimum size:** the full logo should not be used below 120px wide; the mark
  alone not below 24px.
- **Backgrounds:** use the light logo on white/light surfaces and the dark logo
  on `--ht-dark`. Per the style guide, the mark and framing sit on white or
  black backgrounds — **not over images**.
- **Don't:** stretch, rotate, recolour, add effects, or rebuild the wordmark in
  a different font.

## To add

- SVG versions of the full logo (currently PNG only).
- Favicon / app-icon exports (16, 32, 180, 512px).
- Monochrome (single-colour) lock-up for constrained contexts.
