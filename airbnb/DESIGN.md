# Design System: Airbnb

## 1. Visual Theme & Atmosphere

Airbnb's website is a warm, photography-forward marketplace that feels like flipping through a travel magazine where every page invites you to book. The design operates on a foundation of pure white (`#ffffff`) with the iconic Rausch Red (`#ff385c`) — named after Airbnb's first street address — serving as the singular brand accent. The result is a clean, airy canvas where listing photography, category icons, and the red CTA button are the only sources of color.

## 2. Color Palette & Roles

### Primary Brand
- **Rausch Red**: `#ff385c` (primary CTA, brand accent, active states)
- **Deep Rausch**: `#e00b41` (pressed/dark variant)

### Error
- **Error Red**: `#c13515` (error text on light)
- **Error Dark**: `#b32505` (error hover state)

### Premium Tiers
- **Luxe Purple**: `#460479` (Airbnb Luxe tier)
- **Plus Magenta**: `#92174d` (Airbnb Plus tier)

### Text Colors
- **Near Black**: `#222222` (primary text)
- **Focused Gray**: `#3f3f3f` (focused state)
- **Secondary Gray**: `#6a6a6a` (descriptions)
- **Disabled Text**: `rgba(0,0,0,0.24)` (disabled state)
- **Link Disabled**: `#929292`

### Interactive & Surface
- **Legal Blue**: `#428bff` (legal links, informational)
- **Border Gray**: `#c1c1c1` (card dividers)
- **Light Surface**: `#f2f2f2` (nav buttons, secondary)
- **Pure White**: `#ffffff` (background, cards)

## 3. Typography Rules

### Font Family
- **Primary**: Airbnb Cereal VF
- **Fallbacks**: Circular, -apple-system, system-ui, Roboto, Helvetica Neue

### Typography Scale

| Style | Size | Weight | Line Height | Letter Spacing |
|-------|------|--------|-------------|----------------|
| Section Heading | 28px (1.75rem) | 700 | 1.43 | normal |
| Card Heading | 22px (1.38rem) | 600 | 1.18 | -0.44px |
| Card Heading Medium | 22px (1.38rem) | 500 | 1.18 | -0.44px |
| Sub-heading | 21px (1.31rem) | 700 | 1.43 | normal |
| Feature Title | 20px (1.25rem) | 600 | 1.20 | -0.18px |
| UI Medium | 16px (1.00rem) | 500 | 1.25 | normal |
| UI Semibold | 16px (1.00rem) | 600 | 1.25 | normal |
| Button | 16px (1.00rem) | 500 | 1.25 | normal |
| Body / Link | 14px (0.88rem) | 400 | 1.43 | normal |
| Body Medium | 14px (0.88rem) | 500 | 1.29 | normal |
| Caption Salt | 14px (0.88rem) | 600 | 1.43 | normal |
| Small | 13px (0.81rem) | 400 | 1.23 | normal |
| Tag | 12px (0.75rem) | 400-700 | 1.33 | normal |
| Badge | 11px (0.69rem) | 600 | 1.18 | normal |
| Micro Uppercase | 8px (0.50rem) | 700 | 1.25 | 0.32px |

## 4. Component Stylings

### Primary Button (Dark)
- Background: `#222222`
- Text: `#ffffff`
- Padding: 0px 24px
- Radius: 8px
- Focus Ring: `0 0 0 2px` + scale(0.92)

### Circular Navigation Button
- Background: `#f2f2f2`
- Text: `#222222`
- Radius: 50%
- Hover Shadow: `rgba(0,0,0,0.08) 0px 4px 12px`
- Hover Transform: translateX(50%)
- Active Border: 4px white ring
- Focus: scale(0.92)

### Cards & Containers
- Background: `#ffffff`
- Radius: 14px-32px (variable)
- Shadow: Three-layer stack

### Search Input
- Text Color: `#222222`
- Focus Ring: `0 0 0 2px`

## 5. Layout Principles

### Spacing Scale (base unit 8px)
2px, 3px, 4px, 6px, 8px, 10px, 11px, 12px, 15px, 16px, 22px, 24px, 32px

### Grid Architecture
- Desktop (1128-1440px): 4-column listing grid
- Large Desktop (1440-1920px): 5-column grid
- Responsive collapse: 5 -> 4 -> 3 -> 2 -> 1 column progression

## 6. Depth & Elevation

### Card Shadow (Level 1)
`rgba(0,0,0,0.02) 0px 0px 0px 1px, rgba(0,0,0,0.04) 0px 2px 6px, rgba(0,0,0,0.1) 0px 4px 8px`

### Hover Shadow (Level 2)
`rgba(0,0,0,0.08) 0px 4px 12px`

### Focus Ring (Level 3)
`rgb(255,255,255) 0px 0px 0px 4px` + focus ring

## 7. Responsive Behavior

| Name | Width |
|------|-------|
| Mobile Small | <375px |
| Mobile | 375-550px |
| Tablet Small | 550-744px |
| Tablet | 744-950px |
| Desktop Small | 950-1128px |
| Desktop | 1128-1440px |
| Large Desktop | 1440-1920px |
| Ultra-wide | >1920px |

## 8. Border Radius

- **Subtle**: 4px (small links)
- **Standard**: 8px (buttons, tabs, search)
- **Badge**: 14px (status badges, labels)
- **Card**: 20px (feature cards, buttons)
- **Large**: 32px (containers, hero elements)
- **Circle**: 50% (nav controls, avatars)

## 9. Image Treatment

- **Listing photo**: 16:10 ratio
- **Radius**: 8px-14px on contained images; 20px on full-width photo containers
- **Overlay elements**: Heart/wishlist icon positioned consistently
