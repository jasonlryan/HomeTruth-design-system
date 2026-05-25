---
title: Components
type: component-library
category: components
status: scaffold
updated: 2026-05-25
owner: Jason Ryan
tags:
  - design-system
  - component
  - product-ui
---

# Components

Reusable product-UI components, specified once and used everywhere. This folder
is **scaffolded** — specs to be added.

## How to document a component

Each component gets its own Markdown file (e.g. `button.md`) with frontmatter
and these sections:

- **Anatomy** — the parts of the component.
- **Variants** — primary / secondary / etc.
- **States** — default, hover, focus, active, disabled, loading.
- **Tokens used** — the semantic tokens it consumes (never raw primitives).
- **Accessibility** — keyboard, focus, ARIA, contrast, touch-target size.
- **Do / Don't** — short usage guidance.

## Planned components

- `button.md` — primary (orange), secondary, ghost; sizes and states.
- `input.md` — text input, with the waitlist form fields as the reference.
- `card.md` — feature and content cards.
- `nav.md` — top navigation with logo lock-up.
- `badge.md` — status and category tags.

All components must consume semantic tokens from
[`../tokens/tokens.css`](../tokens/tokens.css).
