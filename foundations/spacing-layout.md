---
title: Spacing & Layout
type: foundation
category: foundations
status: stable
updated: 2026-05-25
owner: Jason Ryan
tokens: ../tokens/tokens.json
tags:
  - design-system
  - foundation
  - spacing
  - layout
---

# Spacing & Layout

HomeTruth uses an **8px base grid**. Every margin, padding and gap should be a
multiple of 8 (4px is allowed for fine adjustments). This keeps rhythm
consistent across product UI and marketing pages.

## Spacing scale

| Token | Value |
|-------|-------|
| `--space-0` | 0px |
| `--space-1` | 4px |
| `--space-2` | 8px |
| `--space-3` | 12px |
| `--space-4` | 16px |
| `--space-6` | 24px |
| `--space-8` | 32px |
| `--space-12` | 48px |
| `--space-16` | 64px |
| `--space-24` | 96px |

## Section spacing (from the styleguide)

| Class | Padding |
|-------|---------|
| `.section-y` | `py-16` / `lg:py-24` |
| `.section-y-sm` | `py-12` / `lg:py-16` |

## Radius

| Token | Value |
|-------|-------|
| `--radius-sm` | 4px |
| `--radius-md` | 8px |
| `--radius-lg` | 16px |
| `--radius-full` | 9999px (pills, avatars) |

## Usage notes

- **Vertical rhythm:** use `.section-y` for standard page sections;
  `.section-y-sm` for tighter blocks.
- **Touch targets:** interactive elements should be at least 44×44px.
- **Don't invent values:** if a multiple of 8 doesn't fit, reconsider the
  layout before reaching for an off-grid number.
