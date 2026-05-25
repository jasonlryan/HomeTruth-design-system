---
title: Gradients
type: foundation
category: foundations
status: stable
updated: 2026-05-25
owner: Jason Ryan
tokens: ../tokens/tokens.json
tags:
  - design-system
  - foundation
  - gradient
---

# Gradients

The graduated Orange → Purple → Cyan blend is HomeTruth's signature device. It
ties the three brand colours together and echoes the building-block mark. The
style guide refers to this as the brand "graduation".

## Tokens

| Token | Definition | Direction |
|-------|------------|-----------|
| `--grad-brand` | Orange → Purple → Cyan | 135° (diagonal) |
| `--grad-brand-h` | Orange → Purple → Cyan | 90° (horizontal) |

```css
--grad-brand:   linear-gradient(135deg, var(--ht-orange), var(--ht-purple), var(--ht-cyan));
--grad-brand-h: linear-gradient(90deg,  var(--ht-orange), var(--ht-purple), var(--ht-cyan));
```

## Where to use it

- The top bar / page accent strip.
- Underlines and dividers.
- Gradient text on key headlines (sparingly — one per view).
- Hero and section backgrounds, at low opacity or as an edge accent.

## Usage notes

- **Keep the colour order fixed:** Orange → Purple → Cyan, always.
- **One hero gradient per screen.** Overuse flattens its impact.
- **Contrast:** never place small body text directly on the full-strength
  gradient; reserve it for large display type or decorative elements.
