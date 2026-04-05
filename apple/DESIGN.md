# Design System: Apple

## 1. Visual Theme & Atmosphere

Apple's website exemplifies controlled minimalism — expansive black and near-white backdrops showcase products as gallery sculptures. The design philosophy prioritizes the product absolutely; interface elements recede into invisibility. This represents minimalism as respect for the object itself.

Typography anchors the entire system. San Francisco (SF Pro Display for sizes 20px+, SF Pro Text below) features optical sizing that automatically adjusts letterforms contextually. Display headlines (56px, weight 600, line-height 1.07, letter-spacing -0.28px) feel engineered rather than typeset — precise and authoritative. Body text (17px, line-height 1.47, letter-spacing -0.374px) maintains comfortable readability without appearing loose.

The color approach is starkly binary. Sections alternate between pure black (`#000000`) with white text and light gray (`#f5f5f7`) with near-black text (`#1d1d1f`), creating cinematic pacing. Dark sections convey premium immersion; light sections feel transparent and informational. Apple Blue (`#0071e3`) serves as the solitary chromatic accent, reserved for interactive elements exclusively.

**Key Characteristics:**
- SF Pro with optical sizing — letterforms adapt automatically to size context
- Binary rhythm: black (`#000000`) alternating with light gray (`#f5f5f7`)
- Single accent: Apple Blue (`#0071e3`) for all interactive elements
- Product-as-hero photography on solid color fields only
- Compressed headline line-heights (1.07-1.14) creating billboard impact
- Full-width sections with centered content
- Pill-shaped CTAs (980px radius)
- Generous whitespace between sections

## 2. Color Palette & Roles

### Primary
- **Pure Black** (`#000000`): Hero backgrounds, immersive product showcases
- **Light Gray** (`#f5f5f7`): Alternate sections, informational areas. The blue-gray tint prevents sterility
- **Near Black** (`#1d1d1f`): Primary text on light backgrounds, dark button fills

### Interactive
- **Apple Blue** (`#0071e3`): CTAs, focus rings — THE ONLY chromatic color
- **Link Blue** (`#0066cc`): Inline text links, slightly darker than Apple Blue
- **Bright Blue** (`#2997ff`): Links on dark backgrounds, higher luminance for contrast

### Text
- **White** (`#ffffff`): Text on dark backgrounds, button text
- **Near Black** (`#1d1d1f`): Primary body text on light backgrounds
- **Black 80%** (`rgba(0, 0, 0, 0.8)`): Secondary text, nav items
- **Black 48%** (`rgba(0, 0, 0, 0.48)`): Tertiary text, disabled states

### Surface & Dark Variants
- **Dark Surface 1** (`#272729`): Card backgrounds in dark sections
- **Dark Surface 2** (`#262628`): Subtle variation
- **Dark Surface 3** (`#28282a`): Elevated cards
- **Dark Surface 4** (`#2a2a2d`): Highest elevation
- **Dark Surface 5** (`#242426`): Deepest tone

### Button States
- **Button Active** (`#ededf2`): Pressed state
- **Button Default Light** (`#fafafc`): Search/filter backgrounds
- **Overlay** (`rgba(210, 210, 215, 0.64)`): Media control scrims
- **White 32%** (`rgba(255, 255, 255, 0.32)`): Dark hover states

### Shadows
- **Card Shadow**: `rgba(0, 0, 0, 0.22) 3px 5px 30px 0px` — soft, diffused elevation

## 3. Typography Rules

### Font Family
- **Display**: `SF Pro Display` with fallbacks: `SF Pro Icons, Helvetica Neue, Helvetica, Arial, sans-serif`
- **Body**: `SF Pro Text` with same fallbacks
- Display used at 20px+; Text optimized for 19px and below

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing |
|------|------|------|--------|-------------|----------------|
| Display Hero | SF Pro Display | 56px | 600 | 1.07 | -0.28px |
| Section Heading | SF Pro Display | 40px | 600 | 1.10 | normal |
| Tile Heading | SF Pro Display | 28px | 400 | 1.14 | 0.196px |
| Card Title | SF Pro Display | 21px | 700 | 1.19 | 0.231px |
| Sub-heading | SF Pro Display | 21px | 400 | 1.19 | 0.231px |
| Nav Heading | SF Pro Text | 34px | 600 | 1.47 | -0.374px |
| Sub-nav | SF Pro Text | 24px | 300 | 1.50 | normal |
| Body | SF Pro Text | 17px | 400 | 1.47 | -0.374px |
| Body Emphasis | SF Pro Text | 17px | 600 | 1.24 | -0.374px |
| Button Large | SF Pro Text | 18px | 300 | 1.00 | normal |
| Button | SF Pro Text | 17px | 400 | 2.41 | normal |
| Link | SF Pro Text | 14px | 400 | 1.43 | -0.224px |
| Caption | SF Pro Text | 14px | 400 | 1.29 | -0.224px |
| Caption Bold | SF Pro Text | 14px | 600 | 1.29 | -0.224px |
| Micro | SF Pro Text | 12px | 400 | 1.33 | -0.12px |
| Micro Bold | SF Pro Text | 12px | 600 | 1.33 | -0.12px |
| Nano | SF Pro Text | 10px | 400 | 1.47 | -0.08px |

### Principles
- **Optical sizing**: SF Pro automatically switches between Display and Text. Display versions have wider spacing and thinner strokes; Text versions are tighter and sturdier
- **Weight restraint**: Scale spans 300–700 but primarily uses 400 (regular) and 600 (semibold). Weight 700 appears only on bold card titles
- **Negative tracking universally**: Applies subtle negative letter-spacing at all sizes, creating tight, efficient text
- **Extreme line-height range**: Headlines compress to 1.07; body opens to 1.47; some buttons stretch to 2.41

## 4. Component Stylings

### Buttons

**Primary Blue (CTA)**
- Background: `#0071e3`
- Text: `#ffffff`
- Padding: 8px 15px
- Radius: 8px
- Border: 1px solid transparent
- Font: SF Pro Text, 17px, weight 400
- Hover: background brightens
- Focus: `2px solid #0071e3` outline

**Primary Dark**
- Background: `#1d1d1f`
- Text: `#ffffff`
- Padding: 8px 15px
- Radius: 8px

**Pill Link**
- Background: transparent
- Text: `#0066cc` (light) or `#2997ff` (dark)
- Radius: 980px
- Border: 1px solid `#0066cc`
- Font: SF Pro Text, 14px–17px
- Hover: underline

**Filter / Search Button**
- Background: `#fafafc`
- Text: `rgba(0, 0, 0, 0.8)`
- Padding: 0px 14px
- Radius: 11px
- Border: 3px solid `rgba(0, 0, 0, 0.04)`

**Media Control**
- Background: `rgba(210, 210, 215, 0.64)`
- Text: `rgba(0, 0, 0, 0.48)`
- Radius: 50%

### Cards & Containers
- Background: `#f5f5f7` (light) or `#272729`–`#2a2a2d` (dark)
- Border: none
- Radius: 5px–8px
- Shadow: `rgba(0, 0, 0, 0.22) 3px 5px 30px 0px` for elevated cards
- Content: centered, generous padding

### Navigation
- Background: `rgba(0, 0, 0, 0.8)` with `backdrop-filter: saturate(180%) blur(20px)`
- Height: 48px
- Text: `#ffffff` at 12px, weight 400
- Logo: 17x48px
- Mobile: collapses to hamburger

### Image Treatment
- Products on solid-color fields only
- Full-bleed sections spanning entire viewport width
- High-resolution photography with subtle shadows
- Lifestyle images in rounded containers (12px+ radius)

### Product Hero Module
- Full-viewport-width section with solid background
- Product name as primary headline (56px Display, weight 600)
- One-line descriptor below in lighter weight
- Two pill CTAs: "Learn more" (outline) and "Buy"/"Shop" (filled)

### Product Grid Tile
- Square or near-square card on contrasting background
- Product image dominating 60–70% of tile
- Product name plus one-line description
- "Learn more" and "Shop" links at bottom

### Feature Comparison Strip
- Horizontal scroll of product variants
- Each variant as vertical card with image, name, specs
- Minimal chrome

## 5. Layout Principles

### Spacing System
- Base unit: 8px
- Scale: 2px, 4px, 5px, 6px, 7px, 8px, 9px, 10px, 11px, 14px, 15px, 17px, 20px, 24px
- Dense at small sizes with 1px increments; larger jumps thereafter

### Grid & Container
- Max content width: ~980px
- Hero: full-viewport-width sections with centered content
- Product grids: 2–3 column layouts within centered container
- Single-column for hero moments

### Whitespace Philosophy
- **Cinematic breathing room**: Each section occupies full viewport height (or near). Whitespace between products represents the pause between film scenes
- **Vertical rhythm through color blocks**: Alternating background colors signal new "scenes"
- **Compression within, expansion between**: Text is tightly set; surrounding space is vast, creating tension

### Border Radius Scale
- Micro (5px): Small containers, tags
- Standard (8px): Buttons, product cards, images
- Comfortable (11px): Search inputs, filters
- Large (12px): Feature panels, lifestyle containers
- Full Pill (980px): CTA links, navigation pills
- Circle (50%): Media controls

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat | No shadow, solid background | Standard sections, text |
| Navigation Glass | `backdrop-filter: saturate(180%) blur(20px)` on `rgba(0,0,0,0.8)` | Sticky nav bar |
| Subtle Lift | `rgba(0, 0, 0, 0.22) 3px 5px 30px 0px` | Product cards, floating elements |
| Media Control | `rgba(210, 210, 215, 0.64)` background with scale transforms | Play/pause, carousel |
| Focus | `2px solid #0071e3` outline | Keyboard focus |

**Shadow Philosophy**: Shadows are extremely rare. The primary shadow mimics diffused studio lighting beneath a physical object, reinforcing the "product as sculpture" metaphor. Most elements have no shadow; elevation comes from color contrast.

**Decorative Depth**:
- Navigation glass creates floating UI above scrolling content
- Section color transitions imply depth via alternation
- Product photography shadows replace synthetic UI shadows

## 7. Do's and Don'ts

### Do
- Use SF Pro Display at 20px+, SF Pro Text below — respect optical sizing
- Apply negative letter-spacing at all text sizes universally
- Use Apple Blue (`#0071e3`) ONLY for interactive elements
- Alternate black and `#f5f5f7` section backgrounds for rhythm
- Use 980px radius for CTA links
- Keep product imagery on solid-color fields
- Use translucent dark glass (`rgba(0,0,0,0.8)` + blur) for sticky navigation
- Compress headline line-heights to 1.07–1.14

### Don't
- Don't introduce additional accent colors — blue is the only chromatic element
- Don't use heavy or multiple shadows — one soft diffused shadow or nothing
- Don't use visible borders on cards — they're exceptionally rare
- Don't apply wide letter-spacing to SF Pro
- Don't use weights 800–900 — maximum is 700, and rarely
- Don't add textures, patterns, or gradients to backgrounds
- Don't make navigation opaque — glass blur is essential
- Don't center-align body text — headlines center only
- Don't use rounded corners exceeding 12px on rectangles (980px reserved for pills)

## 8. Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|------|-------|-------------|
| Small Mobile | <360px | Minimum supported, single column |
| Mobile | 360–480px | Standard mobile layout |
| Mobile Large | 480–640px | Wider single column, larger images |
| Tablet Small | 640–834px | 2-column product grids |
| Tablet | 834–1024px | Full tablet layout |
| Desktop Small | 1024–1070px | Desktop layout begins |
| Desktop | 1070–1440px | Full layout, max width |
| Large Desktop | >1440px | Centered with generous margins |

### Touch Targets
- Primary CTAs: 8px 15px padding (~44px touch height)
- Navigation links: 48px height with spacing
- Media controls: 50% radius circular, minimum 44x44px
- Pills: generous padding for comfortable tapping

### Collapsing Strategy
- Hero headlines: 56px Display → 40px → 28px on mobile, maintaining tight line-height proportionally
- Product grids: 3-column → 2-column → stacked
- Navigation: full horizontal → hamburger menu
- Product heroes: full-bleed maintained, text scales down
- Section backgrounds: full-width blocks persist at all sizes
- Images: maintain aspect ratio, never crop — product silhouette is sacred

### Image Behavior
- Product photography maintains aspect ratio
- Hero images scale but stay centered
- Full-bleed section backgrounds persist everywhere
- Lifestyle images may crop on mobile but keep rounded corners
- Lazy loading for below-fold images

## 9. Agent Prompt Guide

### Quick Color Reference
- Primary CTA: Apple Blue (`#0071e3`)
- Page background (light): `#f5f5f7`
- Page background (dark): `#000000`
- Heading text (light): `#1d1d1f`
- Heading text (dark): `#ffffff`
- Body text: `rgba(0, 0, 0, 0.8)` on light, `#ffffff` on dark
- Link (light): `#0066cc`
- Link (dark): `#2997ff`
- Focus ring: `#0071e3`
- Card shadow: `rgba(0, 0, 0, 0.22) 3px 5px 30px 0px`

### Example Component Prompts

**Hero Section**: Create a hero on black background. Headline at 56px SF Pro Display weight 600, line-height 1.07, letter-spacing -0.28px, white text. Subtitle at 21px SF Pro Display weight 400, line-height 1.19, white. Two pill CTAs: "Learn more" (transparent, white text, white border 1px, 980px radius) and "Buy"/"Shop" (`#0071e3` background, white text, 8px radius, 8px 15px padding).

**Product Card**: Design card with `#f5f5f7` background, 8px radius, no border, no shadow. Product image occupies top 60%. Title at 28px SF Pro Display weight 400, letter-spacing 0.196px, line-height 1.14. Description at 14px SF Pro Text weight 400, `rgba(0,0,0,0.8)`. "Learn more" and "Shop" links in `#0066cc` at 14px.

**Apple Navigation**: Sticky, 48px height, `rgba(0,0,0,0.8)` background with `backdrop-filter: saturate(180%) blur(20px)`. Links at 12px SF Pro Text weight 400, white. Apple logo left, links centered, icons right.

**Alternating Sections**: First section black background with white text and centered product image, second section `#f5f5f7` background with `#1d1d1f` text. Each near full-viewport height with 56px headline and two pill CTAs below.

**"Learn more" Link**: Text in `#0066cc` on light backgrounds or `#2997ff` on dark, 14px SF Pro Text, underline on hover. Include right-arrow chevron after text. Wrap in container with 980px border-radius for pill shape when standalone.

### Iteration Guide
1. Every interactive element receives Apple Blue (`#0071e3`) — no alternative accent colors
2. Section backgrounds alternate: black for immersion, `#f5f5f7` for information
3. Typography respects optical sizing: SF Pro Display at 20px+, SF Pro Text below
4. Negative letter-spacing at all sizes: -0.28px (56px), -0.374px (17px), -0.224px (14px), -0.12px (12px)
5. Navigation glass effect (translucent dark + blur) is non-negotiable
6. Products appear on solid color fields only
7. Shadows are rare, always soft: `3px 5px 30px 0.22 opacity` or absent
8. Pill CTAs use 980px radius — signature Apple rounded-rectangle shape
