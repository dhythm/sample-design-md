# IBM Design System: Carbon Design Language

IBM's design approach centers on **enterprise authority through systematic precision**. The Carbon Design System uses a stark visual duality -- white backgrounds with near-black text, anchored by a single accent color: IBM Blue 60 (`#0f62fe`).

## Visual Theme & Atmosphere

IBM's website is the digital embodiment of enterprise authority built on the Carbon Design System. The visual language communicates through systematic precision -- rectangular geometry with 0px border-radius, a monochromatic palette punctuated by a single accent blue, and typography that balances corporate gravitas with unexpected airiness through light-weight display text.

## Color Palette & Roles

### Primary
- IBM Blue 60: `#0f62fe` (singular interactive color)

### Neutral Scale (Gray Family)
- Gray 100: `#161616`
- Gray 90: `#262626`
- Gray 80: `#393939`
- Gray 70: `#525252`
- Gray 60: `#6f6f6f`
- Gray 50: `#8d8d8d`
- Gray 30: `#c6c6c6`
- Gray 20: `#e0e0e0`
- Gray 10: `#f4f4f4`
- Gray 10 Hover: `#e8e8e8`
- White: `#ffffff`

### Interactive
- Blue 60: `#0f62fe`
- Blue 70: `#0043ce`
- Blue 80: `#002d9c`
- Blue 10: `#edf5ff`
- Blue 40: `#78a9ff`

### Support & Status
- Red 60 (Error): `#da1e28`
- Red 70 (Error Hover): `#b81921`
- Green 50 (Success): `#24a148`
- Yellow 30 (Warning): `#f1c21b`

### Focus States
- Focus Blue: `#0f62fe`
- Focus Inset: `#ffffff`

## Typography Rules

IBM Plex Sans at light weight (300) for display headlines creates an unexpectedly airy quality while maintaining corporate gravitas. Monospace needs use IBM Plex Mono with precise letter-spacing.

### Font Family
- Primary: IBM Plex Sans
- Monospace: IBM Plex Mono
- Serif: IBM Plex Serif (editorial/rare use)

### Hierarchy

| Role | Size (px) | Weight | Line Height | Letter Spacing |
|------|-----------|--------|-------------|----------------|
| Display 01 | 60 | 300 | 1.17 | 0px |
| Display 02 | 48 | 300 | 1.17 | 0px |
| Heading 01 | 42 | 300 | 1.19 | 0px |
| Heading 02 | 32 | 400 | 1.25 | 0px |
| Heading 03 | 24 | 400 | 1.33 | 0px |
| Heading 04 | 20 | 400 | 1.40 | 0px |
| Heading 05 | 20 | 600 | 1.40 | 0px |
| Body Long 01 | 16 | 400 | 1.50 | 0px |
| Body Short 01 | 14 | 400 | 1.29 | 0.16px |
| Caption 01 | 12 | 400 | 1.33 | 0.32px |
| Code 01 | 14 | 400 | 1.43 | 0.16px |
| Code 02 | 16 | 400 | 1.50 | 0px |

### Principles
- Light weights (300) at display sizes for expressive headings
- Micro-tracking: 0.16px at 14px, 0.32px at 12px
- Three functional weights only: 300, 400, 600

## Component Stylings

### Buttons
- Height: 48px (default), 40px (compact), 64px (expressive)
- Border-radius: 0px
- Padding: 14px 63px 14px 15px (asymmetric)
- Primary: Blue 60 background, white text
- Secondary: Gray 80 background, white text
- Tertiary: Transparent, Blue 60 border and text
- Ghost: Transparent, Blue 60 text
- Danger: Red 60 background, white text

### Cards & Containers
- Background-color layering for depth (no shadows)
- Surfaces: White, Gray 10 (#f4f4f4), Gray 20 (#e0e0e0)
- Padding: 16px
- Border-radius: 0px

### Inputs & Forms
- Height: 40px (default), 48px (large)
- Bottom-border pattern: 2px solid
- Active/Focus: 2px solid Gray 100 or Blue 60
- Error: 2px solid Red 60

### Navigation
- Height: 48px
- Dark masthead: Gray 100 (#161616) background
- White text, icon-triggered search

### Links
- Default: Blue 60 color
- Hover: underline

## Layout Principles

### Spacing System
- Base unit: 8px (Carbon 2x grid)
- Component scale: 2, 4, 8, 12, 16, 24, 32, 40, 48px
- Layout scale: 16, 24, 32, 48, 64, 80, 96, 160px

### Grid & Container
- 16-column grid (Carbon 2x grid)
- Max content width: 1584px
- Column gutters: 32px (desktop), 16px (mobile)

### Border Radius Scale
- 0px (primary -- buttons, inputs, cards, tiles)
- 2px (small interactive elements)
- 24px (pills/tags)
- 50% (circles -- avatars, icon containers)

## Depth & Elevation

Carbon is deliberately shadow-averse. Depth is achieved through background-color layering.

| Level | Treatment |
|-------|-----------|
| Flat (Level 0) | No shadow |
| Layer 01 | No shadow |
| Layer 02 | No shadow |
| Raised | `0 2px 6px rgba(0,0,0,0.3)` |
| Overlay | `0 2px 6px rgba(0,0,0,0.3)` + dark scrim |

## Responsive Behavior

### Breakpoints

| Name | Width (px) |
|------|-----------|
| Small (sm) | 320 |
| Medium (md) | 672 |
| Large (lg) | 1056 |
| X-Large (xlg) | 1312 |
| Max | 1584 |

### Touch Targets
- Minimum: 48px interactive element sizing

### Collapsing Strategy
- 4-column grids collapse to single columns
- Buttons maintain 48px height across breakpoints
- Responsive typography scales down at smaller viewports
