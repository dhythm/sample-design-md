# Design System: Miro

## 1. Visual Theme & Atmosphere

Clean, collaborative-tool-forward platform that communicates visual thinking through generous whitespace, pastel accent colors, and a confident geometric font.

**Key Characteristics:**
- White canvas with near-black (#1c1c1e) text
- Roobert PRO Medium as the display typeface with OpenType features `"blwf", "cv03", "cv04", "cv09", "cv11"`
- Pastel accent palette with light/dark pairs per section
- Blue 450 (#5b76fe) as primary interactive color
- Success green (#00b473) for positive states
- Border-radius: buttons 8px, cards 12–24px, panels 20–24px, large containers 40–50px
- Framer-built with smooth motion patterns
- Ring shadow as border: `rgb(224,226,232) 0px 0px 0px 1px`

## 2. Color Palette & Roles

### Primary
- Near Black: `#1c1c1e`
- White: `#ffffff`
- Blue 450: `#5b76fe`
- Actionable Pressed: `#2a41b6`

### Pastel Accents (Light / Dark pairs)
- Coral Light: `#ffc6c6` / Coral Dark: `#600000`
- Rose Light: `#ffd8f4`
- Teal Light: `#c3faf5` / Teal Dark: `#187574`
- Orange Light: `#ffe6cd`
- Yellow Dark: `#746019`
- Moss Dark: `#187574`
- Pink: `#fde0f0`
- Red: `#fbd4d4` / Dark Red: `#e3c5c5`

### Semantic
- Success Accent: `#00b473`

### Neutral
- Slate (secondary text): `#555a6a`
- Input Placeholder: `#a5a8b5`
- Border: `#c7cad5`
- Ring Shadow: `rgb(224,226,232) 0px 0px 0px 1px`

## 3. Typography Rules

### Font Families
- **Display:** Roobert PRO (Medium, SemiBold, SemiBold Italic variants), OpenType features: `"blwf", "cv03", "cv04", "cv09", "cv11"`
- **Body:** Noto Sans, Stylistic sets: `"liga" 0, "ss01", "ss04", "ss05"`

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|------|------|------|--------|-------------|----------------|
| Display Hero | Roobert PRO Medium | 56px | 400 | 1.15 | -1.68px |
| Section Heading | Roobert PRO Medium | 48px | 400 | 1.15 | -1.44px |
| Card Title | Roobert PRO Medium | 24px | 400 | 1.15 | -0.72px |
| Sub-heading | Noto Sans | 22px | 400 | 1.35 | -0.44px |
| Feature | Roobert PRO Medium | 18px | 600 | 1.35 | normal |
| Body | Noto Sans | 18px | 400 | 1.45 | normal |
| Body Standard | Noto Sans | 16px | 400–600 | 1.50 | -0.16px |
| Button | Roobert PRO Medium | 17.5px | 700 | 1.29 | 0.175px |
| Caption | Roobert PRO Medium | 14px | 400 | 1.71 | normal |
| Small | Roobert PRO Medium | 12px | 400 | 1.15 | -0.36px |
| Micro Uppercase | Roobert PRO | 10.5px | 400 | 0.90 | uppercase |

## 4. Component Stylings

### Buttons
- **Outlined:** background transparent, border `1px solid #c7cad5`, border-radius 8px, padding 7px 12px, font Roobert PRO Medium 17.5px weight 700, line-height 1.29, letter-spacing 0.175px
- **Primary (Blue):** background `#5b76fe`, color white, pressed state `#2a41b6`
- **White Circle:** border-radius 50%, background white with shadow

### Cards
- Border-radius: 12–24px
- Background: pastel accent colors
- Border: ring shadow `rgb(224,226,232) 0px 0px 0px 1px`

### Inputs
- Placeholder color: `#a5a8b5`
- Border: `#c7cad5`

## 5. Layout Principles

- Spacing scale: 1–24px base increments
- Border-radius hierarchy: buttons 8px → cards 12px → panels 20–24px → large containers 40–50px

## 6. Depth & Elevation

Minimize shadows; use ring borders instead of drop shadows for subtle depth.

## 7. Do's and Don'ts

**Do:**
- Use pastel light/dark pairs per section (max 2 per section)
- Apply OpenType character variants to Roobert PRO
- Use ring shadow as primary border treatment

**Don't:**
- Use heavy drop shadows
- Combine more than 2 pastel accents in a single section

## 8. Responsive Behavior

Breakpoints: 425px, 576px, 768px, 896px, 1024px, 1200px, 1280px, 1366px, 1700px, 1920px

## 9. Agent Prompt Guide

**Quick Color Reference:**
- Background: `#ffffff`
- Text: `#1c1c1e`
- Primary action: `#5b76fe`
- Pressed: `#2a41b6`
- Success: `#00b473`
- Secondary text: `#555a6a`
- Border: `#c7cad5`
