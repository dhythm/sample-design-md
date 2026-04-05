# Design System: Kraken

## 1. Visual Theme & Atmosphere

Kraken's website establishes itself as a trustworthy crypto exchange through clean design centered on purple branding. The aesthetic combines white backgrounds with Kraken Purple variants, employing a dual-font strategy where Kraken-Brand handles display work and Kraken-Product manages interface text.

**Key Characteristics:**
- Purple primary brand color with darker complementary shades
- Dual typography system optimized for hierarchy
- Near-black text paired with cool blue-gray neutrals
- Buttons feature 12-pixel radius (rounded but not fully circular)
- Whisper-level shadows maintaining visual subtlety
- Green accent for success and positive states

## 2. Color Palette & Roles

### Primary
| Hex Code | Name | Purpose |
|----------|------|---------|
| `#7132f5` | Kraken Purple | Primary CTA, brand accent, links |
| `#5741d8` | Purple Dark | Button borders, outlined variants |
| `#5b1ecf` | Purple Deep | Deepest purple shade |
| `rgba(133,91,251,0.16)` | Purple Subtle | Subtle button backgrounds (16% opacity) |

### Text & Neutral Colors
| Hex Code | Name | Purpose |
|----------|------|---------|
| `#101114` | Near Black | Primary text |
| `#686b82` | Cool Gray | Primary neutral, borders at 24% opacity |
| `#9497a9` | Silver Blue | Secondary text, muted elements |
| `#484b5e` | Dark Gray | Badge text (neutral variant) |

### Background & Border Colors
| Hex Code | Name | Purpose |
|----------|------|---------|
| `#ffffff` | White | Primary surface |
| `#dedee5` | Border Gray | Divider borders |
| `rgba(148,151,169,0.08)` | Gray Subtle | Secondary button backgrounds |

### Semantic Colors
| Hex Code | Name | Purpose |
|----------|------|---------|
| `#149e61` | Green | Success/positive states |
| `rgba(20,158,97,0.16)` | Green Subtle | Success badge background (16% opacity) |
| `#026b3f` | Green Dark | Success badge text |

## 3. Typography Rules

### Font Families
- Display: Kraken-Brand (fallbacks: IBM Plex Sans, Helvetica, Arial)
- UI/Body: Kraken-Product (fallbacks: Helvetica Neue, Helvetica, Arial)

### Typographic Scale
| Role | Size | Weight | Line Height | Letter Spacing |
|------|------|--------|-------------|----------------|
| Display Hero | 48px | 700 | 1.17 | -1px |
| Section Heading | 36px | 700 | 1.22 | -0.5px |
| Sub-heading | 28px | 700 | 1.29 | -0.5px |
| Feature Title | 22px | 600 | 1.20 | normal |
| Body | 16px | 400 | 1.38 | normal |
| Body Medium | 16px | 500 | 1.38 | normal |
| Button | 16px | 500-600 | 1.38 | normal |
| Caption | 14px | 400-700 | 1.43-1.71 | normal |
| Small | 12px | 400-500 | 1.33 | normal |
| Micro | 7px | 500 | 1.00 | uppercase |

## 4. Spacing & Layout

### Spacing Scale
1px, 2px, 3px, 4px, 5px, 6px, 8px, 10px, 12px, 13px, 15px, 16px, 20px, 24px, 25px

### Border Radius
3px, 6px, 8px, 10px, 12px, 16px, 9999px, 50%

### Shadows
- Subtle: `rgba(0,0,0,0.03) 0px 4px 24px`
- Micro: `rgba(16,24,40,0.04) 0px 1px 4px`

### Responsive Breakpoints
375px, 425px, 640px, 768px, 1024px, 1280px, 1536px

## 5. Component Specifications

### Buttons

#### Primary Purple
- Background: `#7132f5`
- Text: `#ffffff`
- Padding: 13px 16px
- Border Radius: 12px
- Font: Kraken-Product, 16px, weight 500-600

#### Purple Outlined
- Background: `#ffffff`
- Text: `#5741d8`
- Border: 1px solid `#5741d8`
- Radius: 12px

#### Purple Subtle
- Background: `rgba(133,91,251,0.16)`
- Text: `#7132f5`
- Padding: 8px
- Radius: 12px

#### White Button
- Background: `#ffffff`
- Text: `#101114`
- Radius: 10px
- Shadow: `rgba(0,0,0,0.03) 0px 4px 24px`

#### Secondary Gray
- Background: `rgba(148,151,169,0.08)`
- Text: `#101114`
- Radius: 12px

### Badges

#### Success Badge
- Background: `rgba(20,158,97,0.16)`
- Text: `#026b3f`
- Border Radius: 6px

#### Neutral Badge
- Background: `rgba(104,107,130,0.12)`
- Text: `#484b5e`
- Border Radius: 8px
