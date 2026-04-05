# Pinterest Design System

## Brand Colors

### Primary
- **Pinterest Red**: `#e60023` — Primary CTA, brand accent
- **Green 700**: `#103c25` — Success/nature accent
- **Green 700 Hover**: `#0b2819` — Pressed state

### Text Colors
- **Plum Black**: `#211922` — Primary text
- **Black**: `#000000` — Secondary text, button text
- **Olive Gray**: `#62625b` — Secondary descriptions
- **Warm Silver**: `#91918c` — Disabled text, input borders
- **White**: `#ffffff` — Text on dark surfaces

### Interactive/Accent Colors
- **Focus Blue**: `#435ee5` — Focus rings
- **Performance Purple**: `#6845ab` — Performance features
- **Recommendation Purple**: `#7e238b` — AI recommendations
- **Link Blue**: `#2b48d4` — Link text
- **Facebook Blue**: `#0866ff` — Social login
- **Pressed Blue**: `#617bff` — Pressed state
- **Error Red**: `#9e0a0a` — Form error states

### Surface & Background Colors
- **Sand Gray**: `#e5e5e0` — Secondary button background
- **Warm Light**: `#e0e0d9` — Circular button backgrounds
- **Warm Wash**: `hsla(60, 20%, 98%, 0.5)` — Subtle badge background
- **Fog**: `#f6f6f3` — Light surface
- **Border Disabled**: `#c8c8c1` — Disabled borders
- **Hover Gray**: `#bcbcb3` — Hover border
- **Dark Surface**: `#33332e` — Dark section backgrounds

## Typography

### Font Family
**Primary**: Pin Sans, -apple-system, system-ui, Segoe UI, Roboto, Oxygen-Sans, Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, Helvetica, Arial

### Scale

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 70px (4.38rem) | 600 | normal | normal |
| Section Heading | 28px (1.75rem) | 700 | normal | -1.2px |
| Body | 16px (1.00rem) | 400 | 1.40 | normal |
| Caption Bold | 14px (0.88rem) | 700 | normal | normal |
| Caption | 12px (0.75rem) | 400-500 | 1.50 | normal |
| Button | 12px (0.75rem) | 400 | normal | normal |

## Spacing

**Base Unit:** 8px
**Scale:** 4px, 6px, 7px, 8px, 10px, 11px, 12px, 16px, 18px, 20px, 22px, 24px, 32px, 80px, 100px

## Border Radius

| Application | Value |
|-------------|-------|
| Standard cards | 12px |
| Buttons & inputs | 16px |
| Feature cards | 20px |
| Large containers | 28px |
| Tab elements | 32px |
| Hero containers | 40px |
| Action buttons | 50% (circle) |

## Shadows

- **Level 0 (Flat):** No shadow — default
- **Level 1 (Subtle):** Minimal shadow for overlays
- **Focus State:** Semantic border ring

## Responsive Breakpoints

| Breakpoint | Width |
|------------|-------|
| Mobile | <576px |
| Mobile Large | 576-768px |
| Tablet | 768-890px |
| Desktop Small | 890-1312px |
| Desktop | 1312-1440px |
| Large Desktop | 1440-1680px |
| Ultra-wide | >1680px |

## Components

### Buttons
- **Primary**: bg `#e60023`, text `#000`, padding 6px 14px, radius 16px
- **Secondary**: bg `#e5e5e0`, text `#000`, padding 6px 14px, radius 16px
- **Circular**: bg `#e0e0d9`, radius 50%
- **Ghost**: bg transparent, text `#000`

### Cards
- Border radius: 12px-20px
- Minimal shadow
- Masonry grid layout

### Inputs
- Border: 1px solid `#91918c`
- Border radius: 16px
- Padding: 11px 15px

### Navigation
- Header: white background
- Centered search bar
- Pinterest script mark logo
