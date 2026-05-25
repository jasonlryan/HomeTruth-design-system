---
title: Colour
type: foundation
category: foundations
status: stable
updated: 2026-05-25
owner: Jason Ryan
tokens: ../tokens/tokens.json
provenance: ./brand-provenance.md
tags:
  - design-system
  - foundation
  - colour
---

# Colour

HomeTruth's palette is built from three brand hues, one accent and a neutral
ramp. Colour carries meaning: orange drives action, cyan signals "truth" and
links, purple is the secondary brand voice, green confirms success.

These values are provenance-based decisions. The current operational brand
reference (`BRAND.md`) and implemented token bridge are treated as canonical for
product UI. The BrandAd style-guide PDF names the palette but marks the colour
values as `TBC`, so its swatches are supporting evidence rather than final UI
hex values. See [brand provenance](./brand-provenance.md).

## Primary

| Token | Hex | Use |
|-------|-----|-----|
| `--ht-orange` | `#E8651A` | Primary brand, CTAs, highlights |
| `--ht-orange-light` | `#F28C4E` | Hover / light variant |
| `--ht-cyan` | `#00B4D8` | "Truth" wordmark, links, primary accent |
| `--ht-cyan-light` | `#48D1E8` | Hover / light variant |
| `--ht-purple` | `#8B3FA0` | Secondary brand |
| `--ht-purple-light` | `#A966BF` | Hover / light variant |

## Accent

| Token | Hex | Use |
|-------|-----|-----|
| `--ht-green` | `#43B02A` | Success, positive accent |
| `--ht-green-light` | `#6BC955` | Hover / light variant |

## Neutrals

| Token | Hex | Use |
|-------|-----|-----|
| `--ht-black` | `#1A1A1A` | Text |
| `--ht-dark` | `#0F1620` | Page / section background |
| `--ht-mid-grey` | `#8C8C8C` | Secondary text |
| `--ht-light-grey` | `#C4C4C4` | Borders, muted |
| `--ht-white` | `#FFFFFF` | Body text on dark |

## Aliases (styleguide parity)

| Token | Maps to |
|-------|---------|
| `--ht-primary` | `--ht-cyan` |
| `--ht-secondary` | `--ht-purple` |

## Semantic tokens

Components should reference semantic tokens, not the primitives above:
`--color-action-primary`, `--color-accent`, `--color-secondary`,
`--color-success`, `--color-text-default`, `--color-text-muted`,
`--color-text-on-dark`, `--color-surface-default`, `--color-surface-dark`,
`--color-border-default`. See [`tokens/tokens.css`](../tokens/tokens.css).

## Usage notes

- **Accessibility:** pair text and background for at least WCAG AA contrast
  (4.5:1 for body text). Orange and green should not carry small body text on
  white — use them for fills, CTAs and large elements.
- **Logo artwork colours differ slightly** from these UI tokens. The printed
  brand mark uses orange `#FD6815`, purple `#7B4B9E` and cyan `#19B0F0`. Use
  the UI tokens here for product and web; see [`logos/README.md`](../logos/README.md).
