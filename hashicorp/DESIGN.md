# Design System: HashiCorp

## Visual Theme & Atmosphere

HashiCorp's design system embodies enterprise infrastructure through deliberate visual choices. The system employs a "dual-mode" approach: clean white light-mode for informational sections and a dramatic dark-mode (`#15181e`, `#0d0e12`) for hero areas, reflecting developer workflows.

Token-driven `mds` component system with semantic variable names.

## Color Palette & Roles

### Brand Primary
- `--mds-color-hcp-brand`: `#000000`

### Neutral Scale
- Black: `#000000`
- Dark Charcoal: `#15181e`
- Near Black: `#0d0e12`
- Charcoal: `#3b3d45`
- Dark Gray: `#656a76`
- Cool Gray: `#b2b6bd`
- Mid Gray: `#d5d7db`
- Light Gray: `#f1f2f3`
- Near White: `#efeff1`
- White: `#ffffff`

### Product Brand Colors
- Terraform Purple: `#7b42bc`
- Vault Yellow: `#ffcf25`
- Waypoint Teal: `#14c6cb` (hover: `#12b6bb`)
- Vagrant Blue: `#1868f2`

### Semantic Colors
- Action Blue (dark): `#1060ff`
- Link Blue (light): `#2264d6`
- Bright Blue (active): `#2b89ff`
- Amber: `#bb5a00`
- Amber Light: `#fbeabf`
- Vault Faint Yellow: `#fff9cf`
- Orange: `#a9722e`
- Red: `#731e25`
- Navy: `#101a59`
- Purple Accent: `#911ced`
- Visited Purple: `#a737ff`

### Shadows
- Micro Shadow: `rgba(97, 104, 117, 0.05) 0px 1px 1px, rgba(97, 104, 117, 0.05) 0px 2px 2px`
- Focus Outline: `3px solid var(--mds-color-focus-action-external)`

## Typography Rules

### Font Families
- **Primary Brand**: HashiCorp Sans (`__hashicorpSans_96f0ca`)
- **Fallback**: `__hashicorpSans_Fallback_96f0ca`
- **System Stack**: `system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial`

### Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 82px / 5.13rem | 600 | 1.17 | normal |
| Section Heading | 52px / 3.25rem | 600 | 1.19 | normal |
| Feature Heading | 42px / 2.63rem | 700 | 1.19 | -0.42px |
| Sub-heading | 34px / 2.13rem | 600–700 | 1.18 | normal |
| Card Title | 26px / 1.63rem | 700 | 1.19 | normal |
| Small Title | 19px / 1.19rem | 700 | 1.21 | normal |
| Body Emphasis | 17px / 1.06rem | 600–700 | 1.18–1.35 | normal |
| Body Large | 20px / 1.25rem | 400–600 | 1.50 | normal |
| Body | 16px / 1.00rem | 400–500 | 1.63–1.69 | normal |
| Nav Link | 15px / 0.94rem | 500 | 1.60 | normal |
| Small Body | 14px / 0.88rem | 400–500 | 1.29–1.71 | normal |
| Caption | 13px / 0.81rem | 400–500 | 1.23–1.69 | normal |
| Uppercase Label | 13px / 0.81rem | 600 | 1.69 | 1.3px |

### Principles
- Headings use 600–700 weights with tight line-heights (1.17–1.19), creating dense, authoritative text blocks
- Body text uses system-ui with relaxed line-heights (1.50–1.69)
- All brand typography requires OpenType kerning enabled

## Component Stylings

### Buttons
**Primary Dark:**
- Background: `#15181e`
- Text: `#d5d7db`
- Border: `1px solid rgba(178, 182, 189, 0.4)`
- Radius: `5px`
- Padding: `9px 9px 9px 15px` (asymmetric)
- Hover: `--mds-color-surface-interactive`
- Focus: `3px solid var(--mds-color-focus-action-external)`

**Secondary White:**
- Background: `#ffffff`
- Text: `#3b3d45`
- Padding: `8px 12px`
- Radius: `4px`

### Badges / Pills
- Background: `#42225b`
- Text: `#efeff1`
- Border: `1px solid rgb(180, 87, 255)`
- Padding: `3px 7px`
- Radius: `5px`
- Font: `16px`

### Inputs (Dark Mode)
- Background: `#0d0e12`
- Text: `#efeff1`
- Border: `1px solid rgb(97, 104, 117)`
- Padding: `11px`
- Radius: `5px`
- Helper text: `#656a76`

### Links
- Default: transparent underline → visible on hover
- Light context: `#2264d6`
- Dark context: `#1060ff` or `#2b89ff`
- Hover: `var(--wpl-blue-600)`

### Cards & Containers
- Light: white background with micro-shadow elevation
- Dark: `#15181e` surfaces
- Radius: `8px`

### Navigation
- Nav links: `15px`, weight 500, line-height 1.60

## Layout Principles

### Spacing System
8px base unit: 2px, 3px, 4px, 6px, 7px, 8px, 9px, 11px, 12px, 16px, 20px, 24px, 32px, 40px, 48px

### Grid & Container
- Max content width: ~1150px
- Section vertical spacing: 48px–80px+

### Whitespace Philosophy
- Enterprise breathing room separates sections
- Dense headings, spacious body
- Dark hero sections use extra vertical padding to let illustrations breathe

### Border Radius Scale
- Minimal: `2px`
- Small: `3px`
- Secondary buttons: `4px`
- Primary buttons/badges/inputs: `5px`
- Cards/containers/images: `8px`

## Depth & Elevation

| Level | Shadow | Usage |
|-------|--------|-------|
| 1 – Whisper | `rgba(97,104,117,0.05) 0 1px 1px, rgba(97,104,117,0.05) 0 2px 2px` | Cards, buttons |
| 2 – Focus | `3px solid context-matched-color` | Focus outlines |

## Responsive Behavior

| Breakpoint | Width | Notes |
|------------|-------|-------|
| Mobile Small | <375px | Tight single column |
| Mobile | 375–480px | Standard mobile |
| Small Tablet | 480–600px | Minor tweaks |
| Tablet | 600–768px | 2-column grids begin |
| Small Desktop | 768–992px | Full nav visible |
| Desktop | 992–1120px | Standard layout |
| Large Desktop | 1120–1440px | Max-width content |
| Ultra-wide | >1440px | Centered, generous margins |

**Collapsing Sequence:**
- Headlines scale: 82px → 52px → 42px
- Navigation: mega-menu → hamburger
- Grids: 3-column → 2-column → stacked
- Buttons: inline → full-width stacked (mobile)

## Do's and Don'ts

**Do:**
- Enable kern on all HashiCorp Sans text
- Isolate product colors to respective products
- Use 3px solid focus outlines for accessibility
- Use whisper-level shadows (0.05 opacity)

**Don't:**
- Use cross-product colors
- Exceed 0.1 shadow opacity
- Use pill-shaped buttons (>8px radius)
- Use pure black (#000000) for dark backgrounds
