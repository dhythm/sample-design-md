# Design System: xAI

## 1. Visual Theme & Atmosphere

xAI's website is a masterclass in dark-first, monospace-driven brutalist minimalism -- a design system that feels like it was built by engineers who understand that restraint is the ultimate form of sophistication. The entire experience is anchored to an almost-black background (`#1f2228`) with pure white text (`#ffffff`), creating a high-contrast, terminal-inspired aesthetic that signals deep technical credibility. There are no gradients, no decorative illustrations, no color accents competing for attention. This is a site that communicates through absence.

The typographic system is split between two carefully chosen typefaces. `GeistMono` (Vercel's monospace font) handles display-level headlines at an extraordinary 320px with weight 300, and also serves as the button typeface in uppercase with tracked-out letter-spacing (1.4px). `universalSans` handles all body and secondary heading text with a clean, geometric sans-serif voice. The monospace-as-display-font choice is the defining aesthetic decision -- it positions xAI not as a consumer product but as infrastructure, as something built by people who live in terminals.

The spacing system operates on an 8px base grid with values concentrated at the small end (4px, 8px, 24px, 48px), reflecting a dense, information-focused layout philosophy. Border radius is minimal -- the site barely rounds anything, maintaining sharp, architectural edges. There are no decorative shadows, no gradients, no layered elevation. Depth is communicated purely through contrast and whitespace.

**Key Characteristics:**
- Pure dark theme: `#1f2228` background with `#ffffff` text -- no gray middle ground
- GeistMono at extreme display sizes (320px, weight 300) -- monospace as luxury
- Uppercase monospace buttons with 1.4px letter-spacing -- technical, commanding
- universalSans for body text at 16px/1.5 and headings at 30px/1.2 -- clean contrast
- Zero decorative elements: no shadows, no gradients, no colored accents
- 8px spacing grid with a sparse, deliberate scale
- Heroicons SVG icon system -- minimal, functional
- Tailwind CSS with arbitrary values -- utility-first engineering approach

## 2. Color Palette & Roles

### Primary
- **Pure White** (`#ffffff`): The singular text color, link color, and all foreground elements. In xAI's system, white is not a background -- it is the voice.
- **Dark Background** (`#1f2228`): The canvas. A warm near-black with a subtle blue undertone (not pure black, not neutral gray). This specific hue prevents the harsh eye strain of `#000000` while maintaining deep darkness.

### Interactive
- **White Default** (`#ffffff`): Link and interactive element color in default state.
- **White Muted** (`rgba(255, 255, 255, 0.5)`): Hover state for links -- a deliberate dimming rather than brightening, which is unusual and distinctive.
- **White Subtle** (`rgba(255, 255, 255, 0.2)`): Borders, dividers, and subtle surface treatments.
- **Ring Blue** (`rgb(59, 130, 246) / 0.5`): Tailwind's default focus ring color (`--tw-ring-color`), used for keyboard accessibility focus states.

### Surface & Borders
- **Surface Elevated** (`rgba(255, 255, 255, 0.05)`): Subtle card backgrounds and hover surfaces -- barely visible lift.
- **Surface Hover** (`rgba(255, 255, 255, 0.08)`): Slightly more visible hover state for interactive containers.
- **Border Default** (`rgba(255, 255, 255, 0.1)`): Standard border for cards, dividers, and containers.
- **Border Strong** (`rgba(255, 255, 255, 0.2)`): Emphasized borders for active states and button outlines.

### Functional
- **Text Primary** (`#ffffff`): All headings, body text, labels.
- **Text Secondary** (`rgba(255, 255, 255, 0.7)`): Descriptions, captions, supporting text.
- **Text Tertiary** (`rgba(255, 255, 255, 0.5)`): Muted labels, placeholder text, timestamps.
- **Text Quaternary** (`rgba(255, 255, 255, 0.3)`): Disabled text, very subtle annotations.

## 3. Typography Rules

### Font Family
- **Display / Buttons**: `GeistMono`, with fallback: `ui-monospace, SFMono-Regular, Roboto Mono, Menlo, Monaco, Liberation Mono, DejaVu Sans Mono, Courier New`
- **Body / Headings**: `universalSans`, with fallback: `universalSans Fallback`

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Transform | Notes |
|------|------|------|--------|-------------|----------------|-----------|-------|
| Display Hero | GeistMono | 320px (20rem) | 300 | 1.50 | normal | none | Extreme scale, monospace luxury |
| Section Heading | universalSans | 30px (1.88rem) | 400 | 1.20 (tight) | normal | none | Clean sans-serif contrast |
| Body | universalSans | 16px (1rem) | 400 | 1.50 | normal | none | Standard reading text |
| Button | GeistMono | 14px (0.88rem) | 400 | 1.43 | 1.4px | uppercase | Tracked monospace, commanding |
| Label / Caption | universalSans | 14px (0.88rem) | 400 | 1.50 | normal | none | Supporting text |
| Small / Meta | universalSans | 12px (0.75rem) | 400 | 1.50 | normal | none | Timestamps, footnotes |

### Principles
- **Monospace as display**: GeistMono at 320px is not a gimmick -- it is the brand statement.
- **Light weight at scale**: Weight 300 for the 320px headline prevents the monospace from feeling heavy or brutish at extreme sizes.
- **Uppercase buttons**: All button text is uppercase GeistMono with 1.4px letter-spacing.
- **Sans-serif for reading**: universalSans at 16px/1.5 provides excellent readability for body content.
- **Two-font clarity**: The system uses exactly two typefaces with clear roles.

## 4. Component Stylings

### Buttons

**Primary (White on Dark)**
- Background: `#ffffff`
- Text: `#1f2228`
- Padding: 12px 24px
- Radius: 0px (sharp corners)
- Font: GeistMono 14px weight 400, uppercase, letter-spacing 1.4px
- Hover: `rgba(255, 255, 255, 0.9)` background

**Ghost / Outlined**
- Background: transparent
- Text: `#ffffff`
- Padding: 12px 24px
- Radius: 0px
- Border: `1px solid rgba(255, 255, 255, 0.2)`
- Font: GeistMono 14px weight 400, uppercase, letter-spacing 1.4px
- Hover: `rgba(255, 255, 255, 0.05)` background

**Text Link**
- Background: none
- Text: `#ffffff`
- Font: universalSans 16px weight 400
- Hover: `rgba(255, 255, 255, 0.5)` -- dims on hover

### Cards & Containers
- Background: `rgba(255, 255, 255, 0.03)` or transparent
- Border: `1px solid rgba(255, 255, 255, 0.1)`
- Radius: 0px (sharp) or 4px (subtle)
- Shadow: none
- Hover: border shifts to `rgba(255, 255, 255, 0.2)`

### Navigation
- Dark background matching page (`#1f2228`)
- Brand logotype: white text, left-aligned
- Links: universalSans 14px weight 400, `#ffffff` text
- Hover: `rgba(255, 255, 255, 0.5)` text color
- CTA: white primary button, right-aligned

## 5. Layout Principles

### Spacing System
- Base unit: 8px
- Scale: 4px, 8px, 24px, 48px

### Grid & Container
- Max content width: approximately 1200px
- Hero: full-viewport height with massive centered monospace headline
- Feature sections: simple vertical stacking with generous section padding (48px-96px)

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Flat (Level 0) | No shadow, no border | Page background, body content |
| Surface (Level 1) | `rgba(255,255,255,0.03)` background | Subtle card surfaces |
| Bordered (Level 2) | `1px solid rgba(255,255,255,0.1)` border | Cards, containers, dividers |
| Active (Level 3) | `1px solid rgba(255,255,255,0.2)` border | Hover states, active elements |
| Focus (Accessibility) | `ring` with `rgb(59,130,246)/0.5` | Keyboard focus indicator |

## 7. Do's and Don'ts

### Do
- Use `#1f2228` as universal background
- Use GeistMono for display headlines and button text
- Apply uppercase + 1.4px letter-spacing to all button labels
- Use weight 300 for display headlines
- Keep borders at `rgba(255, 255, 255, 0.1)`
- Dim interactive elements on hover to `rgba(255, 255, 255, 0.5)`
- Maintain sharp corners (0px radius) as default
- Use universalSans for body text at 16px/1.5

### Don't
- Don't use box-shadows
- Don't introduce color accents beyond white and dark background
- Don't use large border-radius (8px+, pill shapes)
- Don't use bold weights (600-700) for headlines
- Don't brighten elements on hover
- Don't add decorative gradients, illustrations, or color blocks
- Don't use proportional fonts for buttons
- Don't use colored status indicators unless functionally necessary
