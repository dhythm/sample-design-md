# Lovable Design System Overview

The Lovable design system creates an approachable, warm digital experience through deliberate choices in color, typography, and component styling.

## Core Visual Identity

The foundation rests on a creamy parchment background (`#f7f4ed`) paired with near-black text (`#1c1c1c`). This isn't minimalism for minimalism's sake -- it's a deliberate choice to feel approachable, almost analog, like a well-crafted notebook.

The Camera Plain Variable typeface -- featuring humanist warmth with organic curves -- differentiates Lovable from typical tech tools. At display sizes (48px-60px), weight 600 with aggressive negative letter-spacing (-0.9px to -1.5px) compresses headlines into confident, editorial statements.

## Color Palette & Roles

### Primary Colors
- **Cream** (`#f7f4ed`): Page background, card surfaces, button surfaces
- **Charcoal** (`#1c1c1c`): Primary text, headings, dark button backgrounds
- **Off-White** (`#fcfbf8`): Button text on dark backgrounds

### Neutral Scale (Opacity-Based on #1c1c1c)
- 100%: `#1c1c1c`
- 83%: `rgba(28,28,28,0.83)` -- Strong secondary text
- 82%: `rgba(28,28,28,0.82)` -- Body copy
- 40%: `rgba(28,28,28,0.4)` -- Interactive borders, button outlines
- 4%: `rgba(28,28,28,0.04)` -- Subtle hover backgrounds
- 3%: `rgba(28,28,28,0.03)` -- Barely-visible overlays

### Surface & Border Colors
- **Light Cream** (`#eceae4`): Card borders, dividers, image outlines
- **Muted Gray** (`#5f5f5d`): Secondary text, descriptions, captions

### Interactive & Focus Colors
- **Ring Blue** (`#3b82f6` at 50% opacity): Tailwind focus ring
- **Focus Shadow** (`rgba(0,0,0,0.1) 0px 4px 12px`): Active/focus states

### Inset Shadow Layers (Buttons)
- White highlight: `rgba(255,255,255,0.2) 0px 0.5px 0px 0px inset`
- Dark ring: `rgba(0,0,0,0.2) 0px 0px 0px 0.5px inset`
- Soft drop: `rgba(0,0,0,0.05) 0px 1px 2px 0px`

## Typography Rules

**Font Family:** Camera Plain Variable (fallback: `ui-sans-serif, system-ui`)

**Weights:** 400 (body/UI), 480 (special display), 600 (headings)

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 60px (3.75rem) | 600 | 1.00-1.10 | -1.5px |
| Display Alt | 60px (3.75rem) | 480 | 1.00 | normal |
| Section Heading | 48px (3rem) | 600 | 1.00 | -1.2px |
| Sub-heading | 36px (2.25rem) | 600 | 1.10 | -0.9px |
| Card Title | 20px (1.25rem) | 400 | 1.25 | normal |
| Body Large | 18px (1.13rem) | 400 | 1.38 | normal |
| Body | 16px (1rem) | 400 | 1.50 | normal |
| Button | 16px (1rem) | 400 | 1.50 | normal |
| Button Small | 14px (0.88rem) | 400 | 1.50 | normal |
| Caption | 14px (0.88rem) | 400 | 1.50 | normal |

**Principles:**
- Negative letter-spacing on headings only (-0.9px to -1.5px)
- Body text: normal tracking for readability
- Two-weight system creates hierarchy through size/spacing, not weight alone

## Spacing System

**Base Unit:** 8px

**Scale:** 8px, 10px, 12px, 16px, 24px, 32px, 40px, 56px, 80px, 96px, 128px, 176px, 192px, 208px

**Philosophy:** Editorial generosity with expansive section boundaries (80-208px vertical) contrasting tight internal card spacing (12-24px). The warm cream background makes these expanses feel cozy rather than empty.

## Component Specifications

### Buttons

**Primary Dark (Inset Shadow)**
- Background: `#1c1c1c`
- Text: `#fcfbf8`
- Padding: 8px 16px
- Radius: 6px
- Shadow: `rgba(255,255,255,0.2) 0px 0.5px 0px 0px inset, rgba(0,0,0,0.2) 0px 0px 0px 0.5px inset, rgba(0,0,0,0.05) 0px 1px 2px 0px`
- Active: opacity 0.8

**Ghost/Outline**
- Background: transparent
- Text: `#1c1c1c`
- Padding: 8px 16px
- Radius: 6px
- Border: `1px solid rgba(28,28,28,0.4)`
- Active: opacity 0.8

### Cards & Containers
- Background: `#f7f4ed` (matches page)
- Border: `1px solid #eceae4`
- Radius: 12px (standard), 16px (featured), 8px (compact)
- No default box-shadow

### Navigation
- Fixed horizontal layout on cream background
- Logo left-aligned
- Links: 14-16px weight 400, `#1c1c1c`
- CTA: dark button with inset shadow, 6px radius
- Mobile: hamburger menu at 768px breakpoint

### Inputs & Forms
- Background: `#f7f4ed`
- Text: `#1c1c1c`
- Border: `1px solid #eceae4`
- Radius: 6px
- Placeholder: `#5f5f5d`

## Border Radius Scale
- **4px:** Small buttons, interactive elements
- **6px:** Buttons, inputs, navigation
- **8px:** Compact cards, divs
- **12px:** Standard cards, image containers
- **16px:** Large containers, footer sections
- **9999px:** Action pills, icon buttons, toggles

## Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (0) | No shadow, cream background | Page surface, most content |
| Bordered (1) | `1px solid #eceae4` | Cards, images, dividers |
| Inset (2) | Multi-layer inset shadow | Dark buttons, primary actions |
| Focus (3) | `rgba(0,0,0,0.1) 0px 4px 12px` | Active/focus states |

## Responsive Breakpoints

| Name | Width | Changes |
|------|-------|---------|
| Mobile | <640px | Single column, reduced padding, hamburger nav |
| Tablet | 640-768px | 2-column grids begin |
| Desktop Small | 768-1024px | Multi-column layouts |
| Desktop | 1024-1280px | Full feature layout |
| Large Desktop | >1280px | Max content width, generous margins |

**Collapsing Strategy:**
- Headlines: 60px -> 48px -> 36px with proportional letter-spacing
- Feature cards: 3-column -> 2-column -> stacked
- Section spacing: 128px+ -> 64px on mobile

## Notable Design Principles

1. Warm parchment background -- a deliberate cream that feels hand-selected
2. Opacity-driven color system ensures tonal unity -- all grays derived from `#1c1c1c` at varying transparency
3. Inset shadows create tactile, pressed-into-surface feeling rather than hovering-above
4. Spacing provides editorial breathing room rather than minimalism
5. Letter-spacing compression at display sizes signals editorial impact
6. No saturated accent colors -- system is warm-neutral by design
