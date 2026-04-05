# Mistral AI Design System Summary

Mistral AI employs a distinctly warm, European-influenced design language centered on golden tones rather than the typical cool blue palette common in tech.

## Core Identity

The system is built around "golden amber, burnt orange, and the feeling of late-afternoon light in southern France." The signature color palette flows from pale cream through amber to burnt orange, with the brand's primary orange (#fa520f) serving as the core identifier.

## Typography Approach

All typography uses weight 400 exclusively—hierarchy derives from size variation rather than weight changes. Display headlines reach 82px with aggressive -2.05px letter-spacing, creating dense, poster-like compositions. This "single weight, maximum impact" strategy means "the entire system uses weight 400 (regular) — even at 82px."

## Color Palette

### Primary Brand Colors
- **Mistral Orange**: `#fa520f` (core brand anchor)
- **Mistral Flame**: `#fb6424` (secondary brand variant)
- **Block Orange**: `#ff8105` (gradient system)

### Sunshine Accent Range
- **Sunshine 900**: `#ff8a00` (deepest golden amber)
- **Sunshine 700**: `#ffa110` (core warm accent)
- **Sunshine 500**: `#ffb83e` (medium golden)
- **Sunshine 300**: `#ffd06a` (light golden)
- **Block Gold**: `#ffe295` (pale gold)
- **Bright Yellow**: `#ffd900` (gradient apex)

### Surface & Background
- **Warm Ivory**: `#fffaeb` (primary page background)
- **Cream**: `#fff0c2` (warm surface)
- **Pure White**: `#ffffff` (maximum contrast)
- **Mistral Black**: `#1f1f1f` (primary dark surface)

### Accent Colors (HSL format)
- **Accent Orange**: `hsl(17, 96%, 52%)`
- **Black Tint**: `hsl(0, 0%, 24%)`
- **Input Border**: `hsl(240, 5.9%, 90%)`
- **White Overlay**: `oklab(1, 0, 0 / 0.088–0.1)`

## Typography System

### Font Stack
Primary: Custom font with fallbacks: `Arial, ui-sans-serif, system-ui, Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol, Noto Color Emoji`

### Type Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display/Hero | 82px (5.13rem) | 400 | 1.00 | -2.05px |
| Section Heading | 56px (3.5rem) | 400 | 0.95 | normal |
| Sub-heading Large | 48px (3rem) | 400 | 0.95 | normal |
| Sub-heading | 32px (2rem) | 400 | 1.15 | normal |
| Card Title | 30px (1.88rem) | 400 | 1.20 | normal |
| Feature Title | 24px (1.5rem) | 400 | 1.33 | normal |
| Body/Button | 16px (1rem) | 400 | 1.50 | normal |
| Caption/Link | 14px (0.88rem) | 400 | 1.43 | normal |

**Key principle**: "Single weight, maximum impact" via size variation exclusively.

## Spacing Scale
Base unit 8px: 2px, 4px, 8px, 10px, 12px, 16px, 20px, 24px, 32px, 40px, 48px, 64px, 80px, 98px, 100px

## Component Specifications

### Buttons
- **Dark Solid**: `#1f1f1f` background, `#ffffff` text, 12px padding
- **Cream Surface**: `#fff0c2` background, `#1f1f1f` text
- **Ghost**: Transparent with `oklab(0, 0, 0 / 0.1)` overlay, 0.4 opacity
- **Text Link**: Transparent, 8px 0px 0px padding

### Cards & Containers
- Background: Warm Ivory, Cream, or Pure White
- Border radius: near-zero (sharp corners)
- Shadow stack: Five cascading amber-tinted layers from 16px to 400px offset using `rgba(127, 99, 21, ...)`

## Shadow System
Primary elevation uses "five cascading layers" of warm amber shadow creating "golden hour" effect:
`rgba(127, 99, 21, 0.12) -8px 16px 39px, rgba(127, 99, 21, 0.1) -33px 64px 72px, rgba(127, 99, 21, 0.06) -73px 144px 97px...`

## Responsive Breakpoints
- Mobile: <640px (hero text: ~32px)
- Tablet: 640–768px
- Small Desktop: 768–1024px
- Desktop: 1024–1280px (full 82px display scale)

## Design Constraints
- No cool colors permitted—exclusively warm spectrum
- Weight 400 only across entire system
- No rounded corners—architectural sharpness required
- Uppercase applied strategically to buttons and section labels
- All shadows must contain amber warmth

## Key Design Elements

- **Color universe**: Exclusively warm tones from pale cream (#fffaeb) to burnt orange (#fa520f)
- **Geometry**: Sharp, architectural corners—near-zero border-radius throughout
- **Shadows**: Five-layered amber-tinted shadows creating "golden hour" lighting effects
- **Photography**: Warm-graded landscape imagery with golden color treatments
- **Buttons**: Primary dark solid (#1f1f1f), secondary cream (#fff0c2), minimal styling overall

## Distinctive Features

The gradient block system (yellow→amber→orange progression) represents the visual DNA, while uppercase typography on CTAs adds formal, European signage quality. The design explicitly avoids cool colors, bold weights, rounded corners, and generic grays—maintaining warmth and architectural precision throughout.
