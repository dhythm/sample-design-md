# SpaceX Design System

## Visual Theme & Atmosphere

The SpaceX design system is a **photographic-first approach** that treats web design as cinema. It operates on pure black (`#000000`) backgrounds with full-viewport aerospace photography. Text overlays sit directly on these photographs with no background panels, cards, or containers — just type on image, bold and unapologetic.

Each section occupies exactly one full viewport (100vh), functioning as individual cinematic scenes. The design explicitly rejects shadows, cards, decorative elements, and traditional containers. The absence of containers IS the design.

## Color Palette & Roles

| Token           | Value                          | Role                        |
|-----------------|--------------------------------|-----------------------------|
| Space Black     | `#000000`                      | Background, void            |
| Spectral White  | `#f0f0fa`                      | Text, near-white            |
| Ghost Surface   | `rgba(240, 240, 250, 0.1)`    | Button background           |
| Ghost Border    | `rgba(240, 240, 250, 0.35)`   | Button outline              |
| Dark Overlay    | `rgba(0, 0, 0, 0.5)`          | Text legibility gradient    |

Achromatic palette only. No accent colors.

## Typography Rules

**Font Family:** D-DIN and D-DIN-Bold exclusively (fallbacks: Arial, Verdana, sans-serif)

| Role            | Size   | Weight | Letter-Spacing | Line-Height |
|-----------------|--------|--------|----------------|-------------|
| Display Hero    | 48px   | 700    | 0.96px         | 1.00        |
| Body            | 16px   | 400    | normal         | 1.50–1.70   |
| Nav Link Bold   | 13px   | 700    | 1.17px         | 0.94        |
| Nav Link        | 12px   | 400    | normal         | 2.00        |
| Caption Bold    | 13px   | 700    | 1.17px         | 0.94        |
| Caption         | 12px   | 400    | normal         | 1.00        |
| Micro           | 10px   | 400    | 1px            | 0.94        |

**Universal rule:** `text-transform: uppercase` applied to nearly all text. This creates an aerospace stencil aesthetic reminiscent of military labeling systems.

## Component Stylings

### Ghost Button (sole interactive element)

- Background: `rgba(240, 240, 250, 0.1)`
- Border: `1px solid rgba(240, 240, 250, 0.35)`
- Padding: 18px
- Border-radius: 32px
- Text color: `#f0f0fa`
- Font: D-DIN-Bold, 13px, uppercase, letter-spacing 1.17px
- Hover: Background brightens, text transitions to full white

### Navigation

- D-DIN 13px, weight 700, uppercase, letter-spacing 1.17px
- Spectral white on transparent overlay
- Logo: 147x19px wordmark
- Mobile: Hamburger collapse pattern

## Layout Principles

- Full-viewport cinematic sections (100vh)
- Edge-to-edge photography (100% width)
- Text overlay on imagery with dark gradient overlay for legibility
- Left-aligned text blocks as primary positioning strategy
- No cards, panels, or traditional containers

### Spacing System

Base unit: 8px
Scale: 3px, 5px, 12px, 15px, 18px, 20px, 24px, 30px

## Depth & Elevation

- Zero shadows throughout the entire system
- No box-shadow, no text-shadow, no drop-shadow
- Depth is conveyed purely through photography and overlay opacity

## Responsive Behavior

| Breakpoint      | Range          |
|-----------------|----------------|
| Mobile          | < 600px        |
| Tablet Small    | 600–960px      |
| Tablet          | 960–1280px     |
| Desktop         | 1280–1350px    |
| Large Desktop   | 1350–1500px    |
| Ultra-wide      | > 1500px       |

Photography maintained full-viewport across all screen sizes.

## Do's and Don'ts

**Do:**
- Use full-bleed photography as the primary visual element
- Keep typography stark and uppercase
- Maintain the achromatic palette
- Let photography create the emotional impact

**Don't:**
- Add shadows, cards, or decorative elements
- Use accent colors or gradients (other than dark overlay)
- Create traditional containers or panels
- Use icons, badges, or dividers
