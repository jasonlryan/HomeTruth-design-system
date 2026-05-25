---
title: HomeTruth Design System
type: design-system
version: 0.1.0
status: draft
updated: 2026-05-25
owner: Jason Ryan
maintainers:
  - Jason Ryan
audience:
  - product
  - ui
  - brand
  - marketing
  - engineering
scope:
  - foundations
  - logos
  - icons
  - components
  - imagery
  - voice-and-tone
brand: HomeTruth
tagline: Your personal property assistant
sources-of-truth:
  - ../hometruth DOCS/BRAND.md
  - ../brand-and-style/HomeTruth Development Style Guide 14.08.pdf
  - https://github.com/jasonlryan/hometruth-styleguide
tags:
  - design-system
  - brand
  - ui
  - design-tokens
---

# HomeTruth Design System

The single, shared reference for how HomeTruth looks, sounds and behaves —
across product UI, brand and marketing. It exists so that anyone building a
screen, a page, a deck or a campaign can reach for the same colours, type,
logos and language without guessing.

> **Status:** `draft` (v0.1.0). Foundations are populated from the
> HomeTruth Development Style Guide (14.08.2025) and `BRAND.md`. Components and
> imagery folders are scaffolded and awaiting content.

## How this is organised

This design system is a folder of plain Markdown, image and token files. The
structure follows the standard design-system layering — **foundations →
assets → components → patterns → voice** — so it stays usable whether you are
in code, in Figma, or writing a brief.

| Folder | What lives here |
|--------|-----------------|
| [`tokens/`](./tokens/) | Machine-readable design tokens — `tokens.json` (W3C DTCG format) and `tokens.css` (CSS custom properties). The source values for everything else. |
| [`foundations/`](./foundations/) | The decisions behind the tokens — [brand provenance](./foundations/brand-provenance.md), [colour](./foundations/colour.md), [typography](./foundations/typography.md), [spacing & layout](./foundations/spacing-layout.md), [gradients](./foundations/gradients.md). |
| [`logos/`](./logos/) | The HomeTruth logo, wordmark and brand mark in all approved forms, plus usage and clear-space rules. |
| [`icons/`](./icons/) | The icon library — building-block symbols and UI icons — with sizing and naming conventions. |
| [`components/`](./components/) | Reusable UI component specs (buttons, inputs, cards, nav). Scaffolded. |
| [`imagery/`](./imagery/) | Photography and illustration direction — wooden building blocks, interior-design features. Scaffolded. |
| [`voice-and-tone/`](./voice-and-tone/) | How HomeTruth writes and speaks. Scaffolded. |

## Token layering

Tokens are organised in the conventional three tiers so the system scales
without colour values being hard-coded into components:

1. **Primitive (base) tokens** — raw values: `--ht-orange: #E8651A`.
2. **Semantic tokens** — intent-based aliases: `--color-action-primary`,
   `--color-text-default`. Components reference these, never the primitives.
3. **Component tokens** — optional, component-scoped: `--button-bg-default`.

When a value changes, change it once in `tokens/` and it flows everywhere.

## Brand at a glance

- **Name & wordmark:** "Home" + "Truth", set in Gill Sans. "Truth" is rendered
  in cyan (`--ht-cyan`).
- **Brand mark:** the "building blocks" symbol — a TH square in orange, purple
  and cyan, representing the smart building blocks of the service.
- **Purpose:** translate complex property information into clear, personalised
  insight so people can buy, manage and improve a home with confidence.
- **Primary palette:** Orange `#E8651A`, Cyan `#00B4D8`, Purple `#8B3FA0`.
- **Accent:** Green `#43B02A` (success / positive).
- **Typeface:** Gill Sans — Light 300, Regular 400, Bold 700.
- **Signature device:** the diagonal Orange → Purple → Cyan gradient.

See [`foundations/colour.md`](./foundations/colour.md) for the full palette and
[`foundations/typography.md`](./foundations/typography.md) for the type scale.

## Using the design system

- **Building product UI:** start from `tokens/tokens.css`, then the
  `foundations/` and `components/` specs.
- **Designing brand or marketing:** start with `logos/`, `foundations/colour.md`,
  `foundations/gradients.md` and `imagery/`.
- **Writing copy:** see `voice-and-tone/`.

## Governance

- **Owner:** Jason Ryan.
- **Source of truth:** brand decisions are made by provenance, not preference.
  See [`foundations/brand-provenance.md`](./foundations/brand-provenance.md)
  for the source hierarchy. Where current references disagree, the digital UI
  palette in `tokens/` is canonical for product, and the logo artwork colours
  are canonical for approved artwork files (see [`logos/README.md`](./logos/README.md)).
- **Changes:** every design-system change must start from a ticket in
  `../HomeTruth-tickets`, include an implementation log in that ticket, be
  referenced by ticket ID in commits or pull requests, and be recorded in
  [`CHANGELOG.md`](./CHANGELOG.md). Bump the `version` in this file's
  frontmatter for canonical token, foundation, component, logo or voice changes
  (semantic versioning).

## Changelog

See [`CHANGELOG.md`](./CHANGELOG.md).
