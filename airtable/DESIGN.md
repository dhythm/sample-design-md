# Airtable Design System

## Core Visual Identity

Airtable employs a "sophisticated simplicity" approach with deep navy text (`#181d26`) on white backgrounds, using Airtable Blue (`#1b61c9`) for interactive elements. The design utilizes the Haas typeface family with consistent positive letter-spacing throughout.

## Color Palette

### Primary Colors
- **Deep Navy**: `#181d26` (primary text)
- **Airtable Blue**: `#1b61c9` (CTAs, links)
- **White**: `#ffffff` (primary surface)
- **Spotlight**: `rgba(249,252,255,0.97)` (button text)

### Semantic Colors
- **Success Green**: `#006400`
- **Weak Text**: `rgba(4,14,32,0.69)`
- **Secondary Active**: `rgba(7,12,20,0.82)`

### Neutral Colors
- **Dark Gray**: `#333333` (secondary text)
- **Mid Blue**: `#254fad` (link variant)
- **Border**: `#e0e2e6` (card borders)
- **Light Surface**: `#f8fafc` (subtle surface)

## Typography System

### Font Families
- **Primary**: Haas (fallbacks: -apple-system, system-ui, Segoe UI, Roboto)
- **Display**: Haas Groot Disp (fallback: Haas)

### Type Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 48px | 400 | 1.15 | normal |
| Display Bold | 48px | 900 | 1.50 | normal |
| Section Heading | 40px | 400 | 1.25 | normal |
| Sub-heading | 32px | 400-500 | 1.15-1.25 | normal |
| Card Title | 24px | 400 | 1.20-1.30 | 0.12px |
| Feature | 20px | 400 | 1.25-1.50 | 0.1px |
| Body | 18px | 400 | 1.35 | 0.18px |
| Body Medium | 16px | 500 | 1.30 | 0.08-0.16px |
| Button | 16px | 500 | 1.25-1.30 | 0.08px |
| Caption | 14px | 400-500 | 1.25-1.35 | 0.07-0.28px |

## Component Specifications

### Buttons
- **Primary Blue**: Background `#1b61c9`, white text, padding 16px 24px, border-radius 12px
- **White**: White background, `#181d26` text, border-radius 12px, 1px white border
- **Cookie Consent**: Background `#1b61c9`, border-radius 2px

### Cards
- Border: 1px solid `#e0e2e6`
- Border-radius: 16px-24px

### Shadow System
- **Blue-tinted multi-layer**: `rgba(0,0,0,0.32) 0px 0px 1px, rgba(0,0,0,0.08) 0px 0px 2px, rgba(45,127,249,0.28) 0px 1px 3px, rgba(0,0,0,0.06) 0px 0px 0px 0.5px inset`
- **Soft ambient**: `rgba(15,48,106,0.05) 0px 0px 20px`

## Spacing & Layout

- **Scale**: 1-48px (8px base unit)
- **Border Radius Values**: 2px (small), 12px (buttons), 16px (cards), 24px (sections), 32px (large), 50% (circles)

## Responsive Breakpoints

- **Range**: 425-1664px
- **Count**: 23 total breakpoints
