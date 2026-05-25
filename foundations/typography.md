---
title: Typography
type: foundation
category: foundations
status: stable
updated: 2026-05-25
owner: Jason Ryan
tokens: ../tokens/tokens.json
tags:
  - design-system
  - foundation
  - typography
---

# Typography

HomeTruth sets everything in **Gill Sans** — a humanist sans-serif that reads
as clear, calm and trustworthy. The wordmark balances Gill Sans weights across
"Home" and "Truth".

## Typeface

- **Family:** Gill Sans
- **Webfont family:** `HomeTruth Gill Sans`
- **Weights:** Light 300, Regular 400, Bold 700
- **Fallback stack:** `"HomeTruth Gill Sans", "Gill Sans", "Gill Sans MT", -apple-system, "Helvetica Neue", Arial, sans-serif`

Token: `--font-base` (see [`tokens/tokens.css`](../tokens/tokens.css)).

The product frontend self-hosts WOFF2 files for Light, Regular and Bold weights
under `public/fonts/`. Confirm web embedding rights before distributing those
font files outside authorised project repositories.

## Type scale

The scale is defined as utility classes in the product `index.html`. Use the
class, not raw font sizes.

| Class | Role |
|-------|------|
| `.type-hero` | Hero / landing headline |
| `.type-h1` | Page title |
| `.type-h2` | Section heading |
| `.type-h3` | Sub-section heading |
| `.type-h4` | Minor heading |
| `.type-body-lg` | Lead / intro paragraph |
| `.type-body` | Default body copy |
| `.type-caption` | Captions, labels, fine print |

## Usage notes

- **Headlines:** Gill Sans Bold (700). Keep them short and confident.
- **Body:** Gill Sans Regular (400) for readability; Light (300) only at large
  sizes — it is too thin for small body text.
- **Emphasis:** prefer weight (Bold) over italics; avoid all-caps for long runs
  of text (the brand uses spaced caps only for the tagline lock-up).
- **Line length:** aim for 60–75 characters for body copy.
