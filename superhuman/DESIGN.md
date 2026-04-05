# Superhuman Design System

## 1. Visual Theme & Atmosphere

Deep purple gradient hero (`#1b1938`) — a deep twilight wash that evokes the moment just before dawn. The typography leverages Super Sans VF, a custom variable font with unconventional weight stops (460, 540, 600, 700). Display text uses ultra-tight 0.96 line-height creating dense, powerful blocks, while body text maintains generous 1.50 line-height for breathing room.

The design philosophy centers on "maximum confidence through minimum decoration."

**Key Characteristics:**
- Deep purple gradient hero (`#1b1938`) contrasting against predominantly white content
- Super Sans VF variable font with non-standard weight stops (460, 540, 600, 700)
- Ultra-tight display line-height (0.96) creating compressed, powerful headlines
- Warm Cream (`#e9e5dd`) buttons — understated luxury instead of bright CTAs
- Lavender Purple (`#cbb7fb`) as singular accent color
- Minimal border-radius scale: only 8px and 16px
- Product screenshots dominate content with minimal surrounding decoration

## 2. Color Palette & Roles

### Primary
- **Mysteria Purple** (`#1b1938`): Hero gradient background
- **Lavender Glow** (`#cbb7fb`): Primary accent and highlight color
- **Charcoal Ink** (`#292827`): Primary text and heading color on light surfaces

### Secondary & Accent
- **Amethyst Link** (`#714cb6`): Underlined link text
- **Translucent White** (`rgba(255, 255, 255, 0.95)`): Hero overlay text
- **Misted White** (`rgba(255, 255, 255, 0.8)`): Secondary text on dark surfaces

### Surface & Background
- **Pure White** (`#ffffff`): Primary page background
- **Warm Cream** (`#e9e5dd`): Button background
- **Parchment Border** (`#dcd7d3`): Card and divider borders

## 3. Typography Rules

### Font Family
- **Display & Body**: `Super Sans VF` (custom variable font)
- Fallbacks: `system-ui, -apple-system, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue`

### Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 64px | 540 | 0.96 | 0px |
| Section Display | 48px | 460 | 0.96 | -1.32px |
| Feature Title | 28px | 540 | 1.14 | -0.63px |
| Card Heading | 22px | 460 | 0.76 | -0.315px |
| Body | 16px | 460 | 1.50 | 0px |
| Button/UI Bold | 16px | 700 | 1.00 | 0px |
| Nav Link | 16px | 460 | 1.20 | 0px |
| Caption | 14px | 500 | 1.20 | -0.315px |

## 4. Component Stylings

### Buttons
- **Warm Cream Primary**: `#e9e5dd` background, `#292827` text, 8px radius, no visible border
- **Dark Primary**: `#292827` background with white text, 8px radius
- **Ghost / Text Link**: No background, underline decoration

### Cards & Containers
- **Content Card**: White background, `#dcd7d3` 1px border, 16px radius
- **Dark Surface Card**: `#292827` border on dark sections
- **Hero Surface**: Semi-transparent white border (`rgba(255, 255, 255, 0.2)`)

### Navigation
- Clean white background on content sections, transparent on hero gradient
- Nav links: 16px, weight 460/600
- CTA button: Warm Cream pill
- Sticky behavior with background transition

## 5. Layout Principles

### Spacing System
- **Base unit**: 8px
- **Scale**: 2px, 4px, 6px, 8px, 12px, 16px, 20px, 24px, 32px, 40px, 48px, 56px
- **Section padding**: 48px-80px vertical
- **Card padding**: 16px-32px

### Grid & Container
- **Max width**: ~1200px content container, centered
- **Column patterns**: Full-width hero, 2-3 column grid for features

### Border Radius
- 8px for buttons and inline elements
- 16px for cards and larger containers

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Level 0 | No shadow, white background | Primary page canvas |
| Level 1 | `1px solid #dcd7d3` | Card containment, dividers |
| Level 2 | `1px solid #292827` | Dark section separators |
| Level 4 | `rgba(255, 255, 255, 0.2)` border | Hero elements |

## 7. Responsive Behavior

### Breakpoints
| Name | Width |
|------|-------|
| Mobile | <768px |
| Tablet | 768px-1024px |
| Desktop | 1024px-1440px |
| Large Desktop | >1440px |

### Font Scaling
- Hero Display: 64px (desktop) -> 48px (tablet) -> 36px (mobile)

## 8. Do's and Don'ts

### Do
- Use weight 460 as default body weight
- Keep display headlines at 0.96 line-height
- Use Warm Cream for primary buttons
- Limit border-radius to 8px and 16px
- Use Lavender Glow as the only accent color
- Let product screenshots be primary visual content

### Don't
- Use conventional font weights (400, 500, 600)
- Add bright or saturated CTA colors
- Introduce additional accent colors
- Apply shadows generously
- Use pure black (`#000000`) for text
- Create pill-shaped buttons
