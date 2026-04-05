# Design System: Clay

## 1. Visual Theme & Atmosphere

Clay's website is a warm, playful celebration of color that treats B2B data enrichment like a craft rather than an enterprise chore. The design language is built on a foundation of warm cream backgrounds (`#faf9f7`) and oat-toned borders (`#dad4c8`, `#eee9df`) that give every surface the tactile quality of handmade paper. Against this artisanal canvas, a vivid swatch palette explodes with personality — Matcha green, Slushie cyan, Lemon gold, Ube purple, Pomegranate pink, Blueberry navy, and Dragonfruit magenta — each named like flavors at a juice bar, not colors in an enterprise UI kit.

The typography is anchored by Roobert, a geometric sans-serif with character, loaded with an extensive set of OpenType stylistic sets (`"ss01"`, `"ss03"`, `"ss10"`, `"ss11"`, `"ss12"`) that give the text a distinctive, slightly quirky personality. At display scale (80px, weight 600), Roobert uses aggressive negative letter-spacing (-3.2px) that compresses headlines into punchy, billboard-like statements. Space Mono serves as the monospace companion for code and technical labels, completing the craft-meets-tech duality.

What makes Clay truly distinctive is its hover micro-animations: buttons on hover rotate slightly (`rotateZ(-8deg)`), translate upward (`translateY(-80%)`), change background to a contrasting swatch color, and cast a hard offset shadow (`rgb(0,0,0) -7px 7px`). This playful hover behavior — where a button literally tilts and jumps on interaction — creates a sense of physical delight that's rare in B2B software. Combined with generously rounded containers (24px–40px radius), dashed borders alongside solid ones, and a multi-layer shadow system that includes inset highlights, Clay feels like a design system that was made by people who genuinely enjoy making things.

**Key Characteristics:**
- Warm cream canvas (`#faf9f7`) with oat-toned borders (`#dad4c8`) — artisanal, not clinical
- Named swatch palette: Matcha, Slushie, Lemon, Ube, Pomegranate, Blueberry, Dragonfruit
- Roobert font with 5 OpenType stylistic sets — quirky geometric character
- Playful hover animations: rotateZ(-8deg) + translateY(-80%) + hard offset shadow
- Space Mono for code and technical labels
- Generous border radius: 24px cards, 40px sections, 1584px pills
- Mixed border styles: solid + dashed in the same interface
- Multi-layer shadow with inset highlight: `0px 1px 1px` + `-1px inset` + `-0.5px`

## 2. Color Palette & Roles

### Primary
- **Clay Black** (`#000000`): Text, headings, pricing card text
- **Pure White** (`#ffffff`): Card backgrounds, button backgrounds, inverse text
- **Warm Cream** (`#faf9f7`): Page background — the warm, paper-like canvas

### Swatch Palette — Named Colors

**Matcha (Green)**
- **Matcha 300** (`#84e7a5`): Light green accent
- **Matcha 600** (`#078a52`): Mid green
- **Matcha 800** (`#02492a`): Deep green for dark sections

**Slushie (Cyan)**
- **Slushie 500** (`#3bd3fd`): Bright cyan accent
- **Slushie 800** (`#0089ad`): Deep teal

**Lemon (Gold)**
- **Lemon 400** (`#f8cc65`): Warm pale gold
- **Lemon 500** (`#fbbd41`): Primary gold
- **Lemon 700** (`#d08a11`): Deep amber
- **Lemon 800** (`#9d6a09`): Dark amber

**Ube (Purple)**
- **Ube 300** (`#c1b0ff`): Soft lavender
- **Ube 800** (`#43089f`): Deep purple
- **Ube 900** (`#32037d`): Darkest purple

**Pomegranate (Pink/Red)**
- **Pomegranate 400** (`#fc7981`): Warm coral-pink

**Blueberry (Navy Blue)**
- **Blueberry 800** (`#01418d`): Deep navy

### Neutral Scale (Warm)
- **Warm Silver** (`#9f9b93`): Secondary/muted text, footer links
- **Warm Charcoal** (`#55534e`): Tertiary text, dark muted links
- **Dark Charcoal** (`#333333`): Link text on light backgrounds

### Surface & Border
- **Oat Border** (`#dad4c8`): Primary border — warm, cream-toned structural lines
- **Oat Light** (`#eee9df`): Secondary lighter border
- **Cool Border** (`#e6e8ec`): Cool-toned border for contrast sections
- **Dark Border** (`#525a69`): Border on dark sections
- **Light Frost** (`#eff1f3`): Subtle button background

### Shadows
- **Clay Shadow** (`rgba(0,0,0,0.1) 0px 1px 1px, rgba(0,0,0,0.04) 0px -1px 1px inset, rgba(0,0,0,0.05) 0px -0.5px 1px`): Multi-layer with inset highlight
- **Hard Offset** (`rgb(0,0,0) -7px 7px`): Hover state — playful hard shadow

## 3. Typography Rules

### Font Families
- **Primary**: `Roobert`, fallback: `Arial`
- **Monospace**: `Space Mono`
- **OpenType Features**: `"ss01"`, `"ss03"`, `"ss10"`, `"ss11"`, `"ss12"` on all Roobert text

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|------|------|------|--------|-------------|----------------|
| Display Hero | Roobert | 80px | 600 | 1.00 | -3.2px |
| Display Secondary | Roobert | 60px | 600 | 1.00 | -2.4px |
| Section Heading | Roobert | 44px | 600 | 1.10 | -0.88px to -1.32px |
| Card Heading | Roobert | 32px | 600 | 1.10 | -0.64px |
| Feature Title | Roobert | 20px | 600 | 1.40 | -0.4px |
| Body Large | Roobert | 20px | 400 | 1.40 | normal |
| Body | Roobert | 18px | 400 | 1.60 | -0.36px |
| Body Standard | Roobert | 16px | 400 | 1.50 | normal |
| Button | Roobert | 16px | 500 | 1.50 | -0.16px |
| Nav Link | Roobert | 15px | 500 | 1.60 | normal |
| Caption | Roobert | 14px | 400 | 1.50 | -0.14px |
| Uppercase Label | Roobert | 12px | 600 | 1.20 | 1.08px |

## 4. Component Stylings

### Buttons
- Primary hover: `rotateZ(-8deg)`, `translateY(-80%)`, hard shadow `rgb(0,0,0) -7px 7px`
- Generous pill radius (1584px) for CTAs
- Ghost outlined: `1px solid #717989`, 4px radius

### Cards & Containers
- Background: `#ffffff` on cream canvas
- Border: `1px solid #dad4c8` (warm oat)
- Radius: 12px (standard), 24px (feature), 40px (sections)
- Shadow: multi-layer with inset highlight

## 5. Layout Principles

### Spacing System
- Base unit: 8px
- Generous breathing room between sections
- Color as spatial rhythm through alternating swatch-colored sections

### Border Radius Scale
- Sharp (4px): Ghost buttons, inputs
- Standard (8px): Small cards
- Card (12px): Standard cards
- Feature (24px): Feature cards, images
- Section (40px): Large sections, footer
- Pill (1584px): CTAs, pill-shaped buttons

## 6. Responsive Behavior

### Breakpoints
| Name | Width |
|------|-------|
| Mobile Small | <479px |
| Mobile | 479-767px |
| Tablet | 768-991px |
| Desktop | 992px+ |
