# Cohere Design System Summary

## Core Visual Identity

Cohere's interface presents itself as "a polished enterprise command deck — confident, clean, and designed to make AI feel like serious infrastructure." The design employs bright white canvases with generously rounded cards (22px radius) that create an organic containment language targeting CTOs and enterprise architects.

## Typography Foundation

The system uses a distinctive dual-typeface approach:
- **CohereText**: Custom display serif for headlines, delivering "the gravitas of a technology manifesto"
- **Unica77 Cohere Web**: Geometric sans-serif for body and UI text, providing "engineering clarity"
- **CohereMono**: Code and technical labels with uppercase transforms

Display text uses negative letter-spacing (-1.44px at 72px) for dense impact, while body text relies on size and spacing rather than weight variation.

### Font Sizes & Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display/Hero | 72px (4.5rem) | 400 | 1.00 | -1.44px |
| Display Secondary | 60px (3.75rem) | 400 | 1.00 | -1.2px |
| Section Heading | 48px (3rem) | 400 | 1.20 | -0.48px |
| Sub-heading | 32px (2rem) | 400 | 1.20 | -0.32px |
| Feature Title | 24px (1.5rem) | 400 | 1.30 | normal |
| Body Large | 18px (1.13rem) | 400 | 1.40 | normal |
| Body/Button | 16px (1rem) | 400 | 1.50 | normal |
| Button Medium | 14px (0.88rem) | 500 | 1.71 | normal |
| Caption | 14px (0.88rem) | 400 | 1.40 | normal |
| Uppercase Label | 14px (0.88rem) | 400 | 1.40 | 0.28px |
| Small | 12px (0.75rem) | 400 | 1.40 | normal |
| Code Micro | 8px (0.5rem) | 400 | 1.40 | 0.16px |

## Color Restraint Strategy

The palette demonstrates extreme chromatic discipline:

### Primary Text Colors
- **Cohere Black**: `#000000` — Primary headline and maximum-emphasis elements
- **Near Black**: `#212121` — Standard body link color
- **Deep Dark**: `#17171c` — Blue-tinted near-black for navigation/dark sections

### Interactive & Accent Colors
- **Interaction Blue**: `#1863dc` — Button hover, focus states, active links
- **Ring Blue**: `#4c6ee6` (50% opacity) — Keyboard focus ring indicator
- **Focus Purple**: `#9b60aa` — Input focus border color

### Surface & Background Colors
- **Pure White**: `#ffffff` — Primary page background and card surface
- **Snow**: `#fafafa` — Elevated surfaces and light-section backgrounds
- **Lightest Gray**: `#f2f2f2` — Card borders and soft containment lines

### Neutral & Border Colors
- **Muted Slate**: `#93939f` — De-emphasized footer links and tertiary text
- **Border Cool**: `#d9d9dd` — Standard section and list-item borders
- **Border Light**: `#e5e7eb` — Lighter border variant (Tailwind gray-200)

### Gradients
- **Purple-Violet Hero Band** — Deep purple gradient full-width sections
- **Dark Footer Gradient** — Deep purple/charcoal transitioning to black footer

## Spacing System

**Base Unit**: 8px

**Scale**: 2px, 6px, 8px, 10px, 12px, 16px, 20px, 22px, 24px, 28px, 32px, 36px, 40px, 56px, 60px

- Card internal padding: 24-32px
- Section vertical spacing: 56-60px between sections
- Max container width: up to 2560px

## Border Radius

- **Sharp (4px)**: Navigation elements, small tags, pagination
- **Comfortable (8px)**: Dialog boxes, secondary containers, small cards
- **Generous (16px)**: Featured containers, medium cards
- **Large (20px)**: Large feature cards
- **Signature (22px)**: Primary cards, hero images, main containers
- **Pill (9999px)**: Buttons, tags, status indicators

## Key Component Principles

### Buttons
- **Ghost/Transparent**: Background transparent, text Cohere Black, hover shifts to Interaction Blue with opacity 0.8
- **Dark Solid**: Dark/black background, white text, for CTAs on light surfaces, pill-shaped
- **Outlined**: Border-based containment for secondary actions

### Cards & Containers
- 22px border-radius signature element
- 1px borders (Lightest Gray or Border Cool) rather than shadows
- White background on purple bands creates elevation without shadows

### Navigation
- Clean horizontal layout on white or dark background
- Text: 16px body font, dark color
- CTA: Dark solid button
- Mobile: Hamburger collapse

### Purple Hero Bands
- Full-width deep purple background sections
- White text content
- Product screenshots float within (22px radius)
- Create dramatic visual breaks

## Depth & Elevation

| Level | Treatment | Usage |
|-------|-----------|-------|
| Flat (Level 0) | No shadow, no border | Page background, text blocks |
| Bordered (Level 1) | 1px solid #f2f2f2 or #d9d9dd | Standard cards, list separators |
| Purple Band (Level 2) | Full-width dark purple background | Hero sections, feature showcases |

## Responsive Breakpoints

- Hero text: 72px -> 48px -> 32px progressive scaling
- Feature grids: 3 columns -> 2 columns -> 1 column
- Navigation: Full -> hamburger
