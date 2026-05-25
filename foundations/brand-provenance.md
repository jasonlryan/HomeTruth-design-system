---
title: Brand Provenance
type: foundation
category: foundations
status: stable
updated: 2026-05-25
owner: Jason Ryan
tags:
  - design-system
  - governance
  - provenance
  - colour
---

# Brand Provenance

Brand decisions must be traceable to source evidence. When sources conflict,
use the highest-ranking source that is explicit, current and fit for the
surface being designed.

## Source Hierarchy

1. **Current operational brand reference**:
   `../../hometruth DOCS/BRAND.md` and `../../hometruth DOCS/CLAUDE.md`.
   These files contain explicit HomeTruth UI token values and are treated as
   canonical for product and web implementation.
2. **Implemented product tokens**:
   `../tokens/tokens.json`, `../tokens/tokens.css` and the frontend token
   bridge in `../../HT_Frontend-staging/src/index.css`. These must mirror the
   operational brand reference.
3. **Brand consultant style guide**:
   `../../brand-and-style/HomeTruth Development Style Guide 14.08.pdf`.
   This establishes brand structure, typography, gradients, logo usage and the
   palette names. Page 10 marks the palette values as `TBC`, so its colour
   swatches are evidence, not final hex decisions.
4. **Logo and artwork assets**:
   `../logos/`, `../icons/` and frontend SVG/PNG artwork. These are canonical
   for the artwork they contain, but their embedded colours should not
   automatically override UI tokens.

## Current Colour Decision

| Role | Decision | Provenance | Notes |
|------|----------|------------|-------|
| HT Orange | `#E8651A` | `BRAND.md`, `CLAUDE.md`, product token bridge | Canonical UI/action colour. |
| HT Purple | `#8B3FA0` | `BRAND.md`, `CLAUDE.md`, product token bridge | Canonical UI secondary colour. |
| HT Cyan | `#00B4D8` | `BRAND.md`, `CLAUDE.md`, product token bridge | Canonical UI accent/link colour and "Truth" wordmark intent. |
| HT Green | `#43B02A` | `BRAND.md`, `CLAUDE.md`, product token bridge | Canonical success/positive accent. |
| Logo orange | `#FD6815` / `#FD6916` sampled | Logo SVG and style-guide swatch | Artwork-only; do not use for UI tokens. |
| Logo purple | `#7B4B9E` / `#7B4C9E` sampled | Logo SVG and style-guide swatch | Artwork-only. The page 7 "Change purple throughout" note is not enough to replace UI purple. |
| Logo cyan/blue | `#19B0F0` / `#00B0F0` sampled | Logo SVG and style-guide swatch | Artwork-only unless a final brand source supersedes the UI token. |
| Style-guide green swatch | `#00D968` sampled | Style-guide page 10 swatch | Evidence only because the page labels green `TBC / Accent Colour`. |

## Decision Rules

- Product UI uses the `ht.*` UI tokens above.
- Logo, favicon and fixed brand artwork use the asset colours embedded in the
  approved artwork files.
- Do not recolour logo artwork to match UI tokens unless a new approved artwork
  file is supplied.
- If a future BrandAd file or message provides final hex values, record the
  source, date and exact wording here before changing tokens.
- If a source says `TBC`, it can support a decision but cannot be the final
  source by itself.
- If two sources conflict at the same hierarchy level, keep the implemented
  token unchanged and open a ticket with the competing evidence.

## Purple Note

The style-guide page 7 note says "Change purple throughout" without specifying
whether it refers to the TH mark, the wordmark, UI tokens or another asset
family. Until a more specific source exists, the decision is:

- keep UI purple as `#8B3FA0`;
- keep the logo/artwork purple embedded in approved assets;
- treat any full-palette purple replacement as a new ticket requiring explicit
  source evidence.
