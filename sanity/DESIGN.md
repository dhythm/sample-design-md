# Sanity Design System Summary

## Core Visual Identity

The system employs **monochromatic discipline with vivid accent punctuation**. The neutral palette ranges from pure black through carefully calibrated grays to white, with no warm or cool bias. Against this achromatic foundation, three accent colors provide signal clarity: coral-red (`#f36458`) for primary CTAs, electric blue (`#0052ef`) as the universal interactive/hover state, and neon green for success indicators.

Typography centers on **waldenburgNormal**, a geometric sans-serif rendered with extreme negative letter-spacing at display scales (up to -4.48px), creating a "precision-cut steel" quality. IBM Plex Mono serves as the technical counterweight for code and labels.

## Key Principles

- **Depth through color, not shadow**: Elevation communicates via surface color shifts (`#0b0b0b` → `#212121` → `#353535`), with borders providing containment
- **Aggressive vertical rhythm**: 64-120px spacing between sections, tighter 16-32px gaps within them
- **Consistent interaction model**: All interactive elements hover to `#0052ef` blue
- **Button morphology**: Primary CTAs use full-pill shape (99999px radius); secondary elements use 3-6px subtle rounding
- **Tight heading hierarchy**: Display text maintains 1.00-1.24 line-height; body text breathes at 1.50

## Responsive Strategy

The design scales deliberately across breakpoints, with hero typography reducing from 112px desktop to 38px mobile while maintaining letter-spacing ratios. Navigation collapses to hamburger below 768px; multi-column grids transition to single-column layouts on smaller screens.

---

## Color Palette

### Primary Brand
- Sanity Black: `#0b0b0b`
- Pure Black: `#000000`
- Sanity Red (CTA): `#f36458`

### Interactive & Accent
- Electric Blue (hover/active): `#0052ef`
- Light Blue variants: `#55beff`, `#afe3ff`
- Neon Green: `#19d600`
- Accent Magenta: `#f500ff`

### Surface & Background
- Dark Gray: `#212121`
- Medium Dark: `#353535`
- Light Gray: `#ededed`
- Pure White: `#ffffff`

### Text
- Primary: `#ffffff`
- Secondary (Silver): `#b9b9b9`
- Tertiary (Medium Gray): `#797979`
- Charcoal: `#212121`

### Semantic
- Error Red: `#dd0000`
- GPC Green: `#37cd84`
- Focus Ring: `#0052ef`

### Borders
- Dark Border: `#0b0b0b`
- Subtle Border: `#212121`
- Medium Border: `#353535`
- Light Border: `#ffffff`

---

## Typography

### Font Families
- Display/Body: waldenburgNormal (fallback: Inter, Space Grotesk)
- Code/Technical: IBM Plex Mono
- CJK: Helvetica, Arial, Hiragino Sans GB

### Font Sizes & Specifications
- Hero: 112px, weight 400, line-height 1.00, tracking -4.48px
- Hero Secondary: 72px, weight 400, line-height 1.05, tracking -2.88px
- Section Heading: 48px, weight 400, line-height 1.08, tracking -1.68px
- Heading Large: 38px, weight 400, line-height 1.10, tracking -1.14px
- Heading Medium: 32px, weight 425, line-height 1.24, tracking -0.32px
- Heading Small: 24px, weight 425, line-height 1.24, tracking -0.24px
- Subheading: 20px, weight 425, line-height 1.13, tracking -0.2px
- Body Large: 18px, weight 400, line-height 1.50, tracking -0.18px
- Body: 16px, weight 400, line-height 1.50
- Body Small: 15px, weight 400, line-height 1.50, tracking -0.15px
- Caption: 13px, weight 400-500, line-height 1.30-1.50, tracking -0.13px
- Small Caption: 12px, weight 400, line-height 1.50, tracking -0.12px
- Micro/Label: 11px, weight 500-600, line-height 1.00-1.50

---

## Spacing System (8px base unit)
- space-1: 1px
- space-2: 2px
- space-3: 4px
- space-4: 6px
- space-5: 8px
- space-6: 12px
- space-7: 16px
- space-8: 24px
- space-9: 32px
- space-10: 48px
- space-11: 64px
- space-12: 96-120px

## Border Radius Scale
- radius-xs: 3px
- radius-sm: 4-5px
- radius-md: 6px
- radius-lg: 12px
- radius-pill: 99999px

---

## Button Specifications

### Primary CTA (Pill)
- Background: `#f36458`
- Text: `#ffffff`
- Padding: 8px 16px
- Radius: 99999px
- Hover: `#0052ef`

### Secondary (Dark Pill)
- Background: `#0b0b0b`
- Text: `#b9b9b9`
- Padding: 8px 12px
- Radius: 99999px
- Hover: `#0052ef`

### Outlined Pill
- Background: `#ffffff`
- Text: `#0b0b0b`
- Padding: 8px
- Radius: 99999px
- Border: 1px solid `#0b0b0b`

### Ghost/Subtle
- Background: `#212121`
- Text: `#b9b9b9`
- Padding: 0px 12px
- Radius: 5px
- Border: 1px solid `#212121`

---

## Card & Container Tokens

### Dark Content Card
- Background: `#212121`
- Border: 1px solid `#353535`
- Radius: 6px
- Padding: 24px

### Feature Card (Full-bleed)
- Background: `#0b0b0b`
- Radius: 12px
- Padding: 32-48px

---

## Input Elements
- Background: `#0b0b0b`
- Border: 1px solid `#212121`
- Radius: 3px
- Padding: 8px 12px
- Focus: 2px solid `#0052ef`

## Shadow System
- Level 0: none
- Level 1: 0px 0px 0px 1px `#212121`
- Level 2: 0 0 0 2px `#0052ef`
