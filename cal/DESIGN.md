# Cal.com Design System

## Visual Theme & Atmosphere

Cal.com's website is a masterclass in monochromatic restraint -- a grayscale world where boldness comes not from color but from the sheer confidence of black text on white space. The design philosophy emphasizes a purely grayscale brand palette with no brand colors, achieving boldness through monochrome.

The elevation approach is shadow-first rather than border-first, utilizing 11 shadow definitions that combine ring borders, diffused shadows, and inset highlights for subtle depth.

## Color Palette

### Primary Text & UI
- **Charcoal**: `#242424` - primary headings, button text, CTA backgrounds
- **Charcoal Alt**: `#1e1f23` - button hover variant
- **Midnight**: `#111111` - deep text, overlays at 50% opacity, nav text
- **Pure Black**: `#000000` - certain link text

### Backgrounds & Surfaces
- **White**: `#ffffff` - primary background, cards, surfaces
- **Light Gray**: `#f5f5f5` - subtle section differentiation

### Secondary Text
- **Mid Gray**: `#898989` - descriptions, secondary labels

### Accent & Interactive
- **Link Blue**: `#0099ff` - hyperlinks with underline
- **Focus Ring**: `#3b82f6` at 50% opacity - keyboard focus, accessibility

### Borders & Shadows (RGBA)
- **Ring Shadow Border**: `rgba(34, 42, 53, 0.08-0.10)`
- **Shadow Dark**: `rgba(19, 19, 22, 0.7)`
- **Shadow Mid**: `rgba(36, 36, 36, 0.7)`
- **Shadow Soft**: `rgba(34, 42, 53, 0.05)`
- **Inset Highlight Light**: `rgba(255, 255, 255, 0.15)`

## Typography

### Font Families
- **Display/Headings**: Cal Sans (custom geometric)
- **Body**: Inter
- **Monospace**: Roboto Mono

### Font Sizes & Hierarchy

| Role              | Font           | Size  | Weight | Line Height | Letter Spacing |
|-------------------|----------------|-------|--------|-------------|----------------|
| Display Hero      | Cal Sans       | 64px  | 600    | 1.10        | 0px            |
| Section Heading   | Cal Sans       | 48px  | 600    | 1.10        | 0px            |
| Feature Heading   | Cal Sans       | 24px  | 600    | 1.30        | 0px            |
| Sub-heading       | Cal Sans       | 20px  | 600    | 1.20        | +0.2px         |
| Body              | Inter          | 16px  | 300    | 1.50        | -0.2px         |
| Caption           | Inter          | 14px  | 500    | 1.14        | 0px            |
| Micro             | Inter          | 12px  | 500    | 1.00        | 0px            |

## Spacing System

- **Base**: 8px
- **Scale**: 1px, 2px, 3px, 4px, 6px, 8px, 12px, 16px, 20px, 24px, 28px, 80px, 96px
- **Section vertical padding**: 80px-96px
- **Card internal padding**: 12px-24px
- **Max-width**: ~1200px

## Border Radius
- **Small**: 4px
- **Medium**: 8px
- **Large**: 12px
- **XL**: 16px
- **Pill**: 9999px

## Shadow System

### Level 2 (Primary Card Shadow)
```
rgba(19,19,22,0.7) 0px 1px 5px -4px,
rgba(34,42,53,0.08) 0px 0px 0px 1px,
rgba(34,42,53,0.05) 0px 4px 8px
```

### Level 4 (Button 3D Effect)
```
rgba(255, 255, 255, 0.15) 0px 2px 0px inset
```

## Components

### Buttons
- **Dark Primary**: `#242424` background, white text, 6-8px radius
- **White/Ghost**: White background, shadow-ring border, dark text
- **Pill**: 9999px radius

### Navigation
- White/transparent background
- Link color: `#111111`
- Sticky on scroll
- Mobile: hamburger menu

## Responsive Breakpoints
- Mobile: <640px
- Tablet: 640-1024px
- Desktop: 1024-1199px
- Large Desktop: >1199px

## Design Principles
- Purely monochromatic (grayscale) brand palette
- Cal Sans (display) + Inter (body) typographic division
- Multi-layered shadow system instead of CSS borders
- Zero gradients; all depth through shadows
- Generous section spacing (80px-96px)
- White canvas with near-black contrast
