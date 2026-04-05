# Mintlify Design System Summary

Mintlify's design system prioritizes clarity and reading comfort through a minimalist approach centered on white backgrounds, near-black text, and a signature green accent (`#18E299`).

## Core Visual Identity

The system employs "a white, airy, information-rich surface that treats clarity as its highest aesthetic value." The palette consists of pure white (`#ffffff`) backgrounds, near-black (`#0d0d0d`) text, and strategic brand green accents. An atmospheric gradient hero featuring "soft, cloud-like green-to-white gradient wash" distinguishes the platform visually.

## Typography Structure

Inter serves as the primary typeface with tight negative tracking at display sizes (-0.8px to -1.28px), while Geist Mono handles technical content exclusively. The hierarchy uses three weights: 400 for body text, 500 for UI elements, and 600 for headings. Body text at 16-18px maintains 150% line-height for reading comfort.

## Component Language

Buttons use "full-pill" styling (9999px radius) consistently across primary dark, secondary ghost, and brand accent variants. Cards feature whisper-thin borders at `rgba(0,0,0,0.05)` opacity with 16-24px radius and generous padding (24px-32px).

## Layout Philosophy

The system emphasizes "documentation-as-product design" with 48px-96px section padding, generous whitespace between elements, and depth created through borders rather than shadows. Maximum content width reaches approximately 1200px with consistent horizontal padding across breakpoints.

---

## CSS Custom Properties

```
--color-brand: #18E299
```

## Color Palette

| Role | Hex |
|------|-----|
| Near Black (Primary Text) | `#0d0d0d` |
| Pure White (Background) | `#ffffff` |
| Brand Green (Accent) | `#18E299` |
| Brand Green Light | `#d4fae8` |
| Brand Green Deep | `#0fa76e` |
| Gray 700 (Secondary Text) | `#333333` |
| Gray 500 (Tertiary Text) | `#666666` |
| Gray 400 (Placeholder) | `#888888` |
| Gray 200 (Borders) | `#e5e5e5` |
| Gray 100 (Subtle Bg) | `#f5f5f5` |
| Gray 50 (Near-white Tint) | `#fafafa` |
| Warm Amber (Warning) | `#c37d0d` |
| Soft Blue (Info) | `#3772cf` |
| Error Red | `#d45656` |

## RGBA Values

- `rgba(0,0,0,0.03)` - ambient shadow
- `rgba(0,0,0,0.05)` - subtle border
- `rgba(0,0,0,0.06)` - button shadow
- `rgba(0,0,0,0.08)` - medium border
- `rgba(255,255,255,0.08)` - dark mode border

## Font Families

- `Inter` (primary); fallback: `Inter Fallback, system-ui, -apple-system, sans-serif`
- `Geist Mono` (monospace); fallback: `Geist Mono Fallback, ui-monospace, SFMono-Regular, monospace`

## Typography Hierarchy

| Element | Size | Weight | Line-height | Letter-spacing | Font |
|---------|------|--------|-------------|----------------|------|
| Display Hero | 64px | 600 | 1.15 | -1.28px | Inter |
| Section Heading | 40px | 600 | 1.10 | -0.8px | Inter |
| Sub-heading | 24px | 500 | 1.30 | -0.24px | Inter |
| Card Title | 20px | 600 | 1.30 | -0.2px | Inter |
| Body Large | 18px | 400 | 1.50 | normal | Inter |
| Body Standard | 16px | 400 | 1.50 | normal | Inter |
| Button Label | 15px | 500 | 1.50 | normal | Inter |
| Caption/Small | 14px | 400-500 | 1.50-1.71 | normal | Inter |
| Label Uppercase | 13px | 500 | 1.50 | 0.65px | Inter |
| Mono Code | 12px | 500-600 | 1.50 | 0.6px | Geist Mono |

## Spacing Scale

2px, 4px, 5px, 6px, 7px, 8px, 10px, 12px, 16px, 24px, 32px, 48px, 64px, 96px

## Border Radius

4px, 8px, 16px, 24px, 9999px

## Buttons

### Primary Brand
- Background: `#0d0d0d`, Text: `#ffffff`
- Padding: 8px 24px, Radius: 9999px
- Font: Inter 15px weight 500
- Shadow: `rgba(0,0,0,0.06) 0px 1px 2px`
- Hover: opacity 0.9

### Secondary / Ghost
- Background: `#ffffff`, Text: `#0d0d0d`
- Padding: 4.5px 12px
- Border: `1px solid rgba(0,0,0,0.08)`, Radius: 9999px
- Hover: opacity 0.9

### Brand Accent
- Background: `#18E299`, Text: `#0d0d0d`
- Padding: 8px 24px, Radius: 9999px

## Cards

### Standard Card
- Background: `#ffffff`
- Border: `1px solid rgba(0,0,0,0.05)`, Radius: 16px
- Padding: 24px
- Shadow: `rgba(0,0,0,0.03) 0px 2px 4px`
- Hover: border darkens to `rgba(0,0,0,0.08)`

### Featured Card
- Radius: 24px, Padding: 32px

## Navigation Bar
- Background: white with `backdrop-filter: blur(12px)`
- Position: sticky
- Border-bottom: `1px solid rgba(0,0,0,0.05)`
- Links: Inter 14-15px weight 500
- Mobile: hamburger at 768px

## Responsive Breakpoints

| Breakpoint | Width | Layout |
|------------|-------|--------|
| Mobile | <768px | Single column, hamburger nav, 48px section padding |
| Tablet | 768-1024px | Two-column grids |
| Desktop | >1024px | Full layout, 3-column grids, 96px section padding |
