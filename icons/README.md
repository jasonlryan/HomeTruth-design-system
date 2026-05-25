---
title: Icons
type: asset-library
category: icons
status: draft
updated: 2026-05-25
owner: Jason Ryan
tags:
  - design-system
  - icon
assets:
  - hometruth-icon.svg
  - icon-lifecycle-purchase.svg
  - icon-lifecycle-maintain.svg
  - icon-lifecycle-improve.svg
  - icon-lifecycle-sell.svg
---

# Icons

HomeTruth's iconography draws on the **building-block** language of the brand
mark. Icons should feel constructed, geometric and calm — the same family as
the framing symbols in the style guide.

## Files in this folder

| File | Format | Use |
|------|--------|-----|
| `hometruth-icon.svg` | SVG | The building-block brand mark — also used as the master icon reference |
| `icon-lifecycle-purchase.svg` | SVG | Purchase stage framing/icon motif |
| `icon-lifecycle-maintain.svg` | SVG | Maintain stage framing/icon motif |
| `icon-lifecycle-improve.svg` | SVG | Improve stage framing/icon motif |
| `icon-lifecycle-sell.svg` | SVG | Sell stage framing/icon motif |

## Sizing

Icon sizes are anchored to the 8px grid. Use the size tokens, not arbitrary
values.

| Token | Size | Typical use |
|-------|------|-------------|
| `--icon-size-sm` | 16px | Inline with body text, dense UI |
| `--icon-size-md` | 24px | Navigation, buttons, default UI |
| `--icon-size-lg` | 32px | Feature blocks, headers |

Draw icons on a 24×24px artboard with a consistent stroke; scale from there.

## Naming convention

Use lowercase, hyphenated names with a category prefix so the library stays
sortable and predictable:

```
icon-[category]-[name]-[variant]
```

Examples: `icon-nav-home`, `icon-nav-home-filled`, `icon-action-search`,
`icon-status-success`, `icon-property-document`.

## Colour

- Icons reference semantic colour tokens — e.g. `fill: var(--color-text-muted)`
  or `var(--color-accent)` — never hard-coded hex values.
- Default UI icons are monochrome; reserve multi-colour for the brand mark.

## To add

- A full UI icon set (navigation, actions, status, property/home concepts).
- The "icon dial" device from the style guide.
- An `icons/svg/` subfolder once the set grows beyond a handful of files.
