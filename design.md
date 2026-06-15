# Design System Inspired by Spanish Mission Architecture

## 1. Visual Theme & Atmosphere

A Spanish Mission interface is an exercise in warm restraint — a digital courtyard where hand-wrought surfaces, arched openings, and sun-baked color carry the experience. The page opens with a full-viewport hero filled with atmospheric mission imagery: whitewashed adobe walls glowing in late-afternoon light, a red terracotta roofline against a deep blue sky, bougainvillea spilling over a wrought-iron balcony. Decorative detail exists, but it is always earned: a hand-painted tile border, a carved wooden corbel, an iron lantern catching the light. The interface frames the content like a shaded arcade around a central fountain — generous, breathable, and quietly ornate.

The color philosophy is grounded in the landscape of the American Southwest and Mediterranean coast: warm plaster whites, terracotta roof tiles, sage and cactus greens, deep cobalt accents, and weathered iron browns. Surfaces read as tactile even on screen — stucco texture, Saltillo tile patterns, aged wood grain. The navigation bar floats above the hero like a white adobe lintel, its background shifting from transparent over imagery to an opaque plaster white on scroll. There are no harsh gradients, no neon accents, no cold grays. Every color feels as though it has been faded by a century of sun.

Typography draws from hand-lettered mission signage and contemporary Southwestern editorial design. Headlines are set in a warm, humanist serif or a softly geometric slab (inspired by carved mission plaques and vintage travel posters), while body and UI text use a clean, highly legible sans-serif with gently rounded terminals. Headlines may carry a subtle texture or letterpress quality, but never at the expense of readability. Decorative type is reserved for small labels and accents — a single hand-drawn flourish, a small cross, or a mission bell icon — never for primary navigation or CTAs.

**Key Characteristics:**
- Full-viewport hero sections (100vh) dominated by warm, sunlit mission photography with minimal overlay UI
- Arched shapes and rounded openings as the default decorative motif — softened corners, arch-top cards, semicircular buttons
- Warm, earth-toned palette: plaster white, terracotta, sage green, cobalt blue, aged iron, golden ochre
- Textured surfaces that read as stucco, tile, wood, or wrought iron
- Talavera tile and hand-painted pattern accents used sparingly as borders or small medallions
- Photography-first presentation where courtyards, arches, tile, and landscape carry emotional weight
- Adobe-plaster navigation concept that floats over hero imagery and turns opaque white on scroll
- 0.4s ease-in-out transitions as the universal timing for interactive state changes
- Carousel-driven hero with dot indicators and edge arrow navigation for multiple mission showcases
- "Plan a Visit" persistent concierge bar anchored to the viewport bottom

## 2. Color Palette & Roles

### Primary
- **Terracotta** (`#C25E3D`): Primary CTA button background — a warm, sun-fired clay red (rgb 194, 94, 61) that echoes roof tiles and pottery. Used exclusively for "Plan a Visit" and other primary action buttons
- **Plaster White** (`#F7F4EF`): Dominant background color for all surfaces, panels, navigation, and secondary button fills — the warm, creamy canvas that lets photography and tile breathe

### Secondary & Accent
- **Cobalt Accent** (`#1E4D8C`): Deep Mediterranean blue for promotional text ("Free Guided Tours") and small decorative accents — used sparingly to mirror the bright blue sky and painted tile details
- **Sage Green** (`#7A8B6E`): Secondary accent for nature, garden, and sustainability messaging — drawn from cactus, olive, and agave tones
- **Golden Ochre** (`#D4A35A`): Warm highlight for seasonal badges, small decorative icons, and emphasis text — like sun on adobe walls

### Surface & Background
- **Plaster White** (`#F7F4EF`): Page background, navigation panel, dropdown menus, and all surface containers — warm, not stark
- **Adobe Sand** (`#E8E0D5`): Subtle alternate surface for section differentiation — a warm beige shift from plaster white (rgb 232, 224, 213)
- **Mission Brown** (`#5C4033`): Dark surface color for hero text overlays and footer areas (rgb 92, 64, 51) — a warm, weathered wood brown
- **Frosted Plaster** (`rgba(247, 244, 239, 0.85)`): Semi-transparent warm white for navigation backdrop-filter effects on scroll

### Neutrals & Text
- **Mission Brown** (`#5C4033`): Primary heading and navigation text — the darkest text value (rgb 92, 64, 51), used for section titles, nav labels, and hero titles on light backgrounds
- **Adobe Graphite** (`#4A4540`): Body text and secondary content (rgb 74, 69, 64) — a warm, earthy gray-brown
- **Wrought Iron** (`#6E665F`): Tertiary text for sub-links, secondary navigation links like "Explore" and "Reserve" (rgb 110, 102, 95)
- **Dust Gray** (`#A8A199`): Placeholder text in input fields and disabled states (rgb 168, 161, 153)
- **Clay Border** (`#D9CFC2`): Light borders and divider lines (rgb 217, 207, 194)
- **Tile Cream** (`#E6DCCF`): Subtle UI borders and delineation (rgb 230, 220, 207)

### Semantic & Accent
- Spanish Mission sites favor warm, natural signals over clinical semantic colors
- The terracotta CTA (`#C25E3D`) serves as the primary interactive color signal
- Success states may use Sage Green (`#7A8B6E`); error states use a muted brick red (`#A84A3B`); warnings use Golden Ochre (`#D4A35A`)

### Gradient System
- No gradients are used anywhere in the interface
- Depth is achieved entirely through photography, texture, and the contrast between warm white surfaces and sun-drenched imagery
- The navigation achieves layering through warm opacity (frosted plaster effect) rather than gradient or shadow

## 3. Typography Rules

### Font Family
- **Display**: `Crimson Pro`, `Playfair Display`, Georgia, serif — used for hero titles and large section names. A warm, humanist serif with classic proportions, evoking carved mission inscriptions and vintage travel posters
- **Text/UI**: `Source Sans 3`, `Nunito Sans`, -apple-system, Arial, sans-serif — used for navigation, body copy, buttons, and all UI text. Optimized for legibility with slightly rounded, friendly terminals
- **Accent**: `Permanent Marker` or a custom hand-lettered style — used very sparingly for small decorative labels, stamp-like badges, or "Est. 1776" details
- **No uppercase transforms** for body or UI — the lowercase approach reinforces the relaxed, sun-warmed personality

### Hierarchy

| Role | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|--------|-------------|----------------|-------|
| Hero Title | 42px (2.625rem) | 600 | 50px (1.19) | -0.01em | Display serif, Plaster White or Mission Brown on warm hero imagery |
| Product Name | 18px (1.125rem) | 600 | 22px (1.22) | normal | Sans-serif, model/location names in cards and panels |
| Nav Item | 14px (0.875rem) | 600 | 17px (1.21) | 0.02em | Sans-serif, primary navigation labels, slight tracking |
| Body Text | 15px (0.9375rem) | 400 | 24px (1.60) | normal | Sans-serif, paragraph and descriptive content — generous line height |
| Button Label | 14px (0.875rem) | 600 | 17px (1.21) | 0.04em | Sans-serif, CTA button text, slight tracking |
| Sub-link | 14px (0.875rem) | 400 | 20px (1.43) | normal | Tertiary links (Explore, Reserve, History) |
| Promo Text | 22px (1.375rem) | 400 | 24px (1.09) | normal | Promotional text on hero ("Free Guided Tours") |
| Category Label | 16px (1rem) | 600 | — | 0.02em | White or warm text labels on category cards ("Courtyards", "Tile Work") |

### Principles
- **Slight negative tracking on large serif headlines only**: Hero titles use a subtle -0.01em to tighten the classical serif forms; all other text uses default or slight positive tracking
- **Weight restraint**: 400 (regular) for body, 600 (semibold) for headings and UI. No extreme bold (800+) or light (300) weights
- **Generous body line height**: 1.6 line height on body copy reflects the airy, courtyard-like spacing of the layout
- **Display vs Text split**: Serif for hero and section headlines, sans-serif for everything functional
- **No text transforms** in navigation or CTAs — lowercase calm, with slight tracking for nav and buttons only

## 4. Component Stylings

### Buttons
All buttons use softly rounded rectangles (8px border-radius) or pill shapes — echoing arched doorways and rounded tile edges rather than sharp modern corners.

**Primary CTA** — The main action button:
- Default: bg `#C25E3D` (Terracotta), text `#F7F4EF` (Plaster White), fontSize 14px, fontWeight 600, padding 4px with inner content centering, borderRadius 8px, minHeight 44px, width 220px
- Border: 2px solid transparent (reserves space for focus/active border)
- Box Shadow: `rgba(0,0,0,0) 0px 0px 0px 2px inset` (invisible at rest, animates to visible on focus)
- Transition: `border-color 0.4s, background-color 0.4s, color 0.4s, box-shadow 0.3s`
- Hover: subtle darkening of terracotta background
- Used for: "Plan a Visit" calls to action

**Secondary CTA** — The alternative action button:
- Default: bg `#F7F4EF` (Plaster White), text `#4A4540` (Adobe Graphite), same dimensions and border pattern as primary
- Transition: identical timing to primary (0.4s)
- Used for: "View Events" alongside primary CTA

**Nav Button** — Top navigation items:
- Default: bg transparent, text `#5C4033` (Mission Brown), fontSize 14px, fontWeight 600, letterSpacing 0.02em, borderRadius 8px, padding 6px 16px, minHeight 36px
- Transition: `color 0.4s, background-color 0.4s`
- Active/expanded: subtle Adobe Sand background highlight
- Used for: "Explore", "History", "Visit", "Events", "Shop"

**Text Link** — In-content actions:
- Default: text `#6E665F` (Wrought Iron), fontSize 14px, fontWeight 400, no background, no border
- Hover: underline decoration with box-shadow transition
- Transition: `box-shadow 0.4s ease-in-out, color 0.4s`
- Used for: "Explore", "Reserve", "History", "New", "Gift Shop" links in dropdown panel

### Cards & Containers

**Experience Card** (Navigation panel):
- Background: transparent (inherits panel plaster white)
- Border: 1px solid `#D9CFC2` (Clay Border) — optional, used only where separation is needed
- Shadow: none
- Content: mission image + experience name centered below + two text links
- Layout: 3-column grid within the dropdown panel
- No hover animation on the card itself — interaction is via the text links beneath

**Category Card** (Homepage lower section):
- Background: full-bleed mission photography or warm texture
- Border radius: 16px top corners with a gentle arch effect, 12px bottom corners — evoking arched doorways
- Overflow: hidden (clips image to rounded corners)
- Text: warm label in top-left corner ("Courtyards", "Tile Work")
- Size: large format, approximately 2:1 aspect ratio
- No shadow, no overlay gradient — text relies on image warmth and contrast

### Inputs & Forms
- Background: `#F7F4EF` (Plaster White)
- Text color: `#5C4033` (Mission Brown)
- Placeholder color: `#A8A199` (Dust Gray)
- Border: 1px solid `#D9CFC2` (Clay Border), borderRadius 8px
- Font: Sans-serif, 14px
- The "Plan a Visit" concierge input bar sits at the viewport bottom with a warm white background and subtle clay border

### Navigation
- **Desktop**: Centered horizontal nav with a mission wordmark or simple icon on the left, five category buttons center-aligned, and three icon buttons (help, language, account) on the right
- **Background**: Plaster White (transitions from transparent over dark hero to opaque warm white on scroll via class toggle `mission-site-header--plaster-background`)
- **Dropdown panel**: Full-width warm white panel with 3-column experience grid + right sidebar text links, no heavy shadow, subtle clay border top — appears seamlessly below the nav
- **Sticky behavior**: `sticky-without-slide` class — stays at top without slide-in animation
- **Mobile**: Hamburger collapse pattern with arched-top drawer
- **No visible separator** between nav and content — the nav blends with the hero

### Image Treatment
- **Hero**: Full-viewport (100vh) sections with warm mission photography — edge-to-edge, no padding, no margin
- **Mission images**: Warm, sunlit photography on plaster-white backgrounds in dropdown panels
- **Category cards**: Landscape photography with approximately 2:1 ratio, arched top corners (16px) and rounded bottom corners (12px)
- **Carousel**: Auto-advancing with dot indicators and left/right arrow navigation on edges
- **Lazy loading**: Below-fold sections use lazy loading, rendering as warm white until scrolled into view

### Persistent Concierge Bar
- Anchored to viewport bottom, visible across all sections
- Plaster White background with subtle Clay Border top
- Contains: concierge icon + "Plan a Visit" label + placeholder text ("What would you like to explore?") + send icon + "View Upcoming Events" secondary CTA
- Events CTA has a small Golden Ochre or Sage Green icon accent

## 5. Layout Principles

### Spacing System
- **Base unit**: 8px
- **Common values**: 8px (0.5rem), 16px (1rem), 24px (1.5rem), 32px (2rem)
- **Button padding**: 4px (minimal outer) with content centering via flexbox, 6px 16px for nav items
- **Section padding**: Full-viewport sections with content centered vertically
- **Card gap**: approximately 16px between category cards

### Grid & Container
- **Max width**: approximately 1280px (full viewport width used for most content)
- **Hero**: Full-bleed, edge-to-edge, 100vh sections
- **Navigation panel**: 3-column grid for experience cards with right-aligned text sidebar (~70/30 split)
- **Category cards**: 2-up horizontal layout (large left card + smaller right card)

### Whitespace Philosophy
Spanish Mission design uses whitespace as a courtyard — open, breathable, and intentional. The generous vertical spacing between sections (each major section is a full viewport height) means you encounter one "room" at a time: one courtyard, one chapel interior, one tiled fountain. This creates a procession-like browsing experience where each scroll is a deliberate transition through arched openings. White space is not empty — it's the shaded arcade that frames each sunlit scene.

### Border Radius Scale
| Value | Context |
|-------|---------|
| 0px | Most structural elements — sharp edges are rare |
| 8px | Buttons (primary, secondary, nav items) — softly rounded |
| 12px | Small cards, inputs, and containers |
| 16px / arch | Category cards — arched top corners evoking mission doorways |
| 50% | Carousel dot indicators and circular icon buttons — perfect circles |

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Level 0 (Flat) | No shadow, no border | Default state for most elements — cards, panels, buttons at rest |
| Level 1 (Frost) | `rgba(247,244,239,0.85)` backdrop | Navigation bar on scroll — frosted plaster transparency |
| Level 2 (Overlay) | `rgba(92,64,51,0.55)` | Modal overlays and region/cookie popups — warm brown tint |
| Level 3 (Subtle) | `rgba(0,0,0,0.06)` | Minimal shadow hints on rare hover states |

### Shadow Philosophy
Spanish Mission design avoids heavy, modern box-shadows. Depth is communicated through three alternative strategies:
1. **Z-index layering**: The sticky navigation sits above hero content through positioning, not shadow
2. **Opacity-based transparency**: The frosted plaster nav and overlay modals use background-color opacity rather than shadow to indicate layering
3. **Photography and texture as depth**: Sunlit walls, recessed arches, and wrought-iron grilles create their own visual depth — making UI shadows redundant

### Decorative Depth
- No gradients, glows, or atmospheric effects on UI elements
- The hero imagery and texture provide all visual richness — whitewashed stucco, terracotta roofs, painted tiles, iron scrollwork
- The carousel arrow buttons use a semi-transparent Plaster White background to float above the hero imagery without disrupting it

## 7. Do's and Don'ts

### Do
- Let warm mission photography dominate every screen — the place IS the design
- Use Terracotta (`#C25E3D`) exclusively for primary CTAs — never for decorative purposes
- Maintain viewport-height sections for major content blocks — one message per screen
- Keep typography at weight 400-600 only — no extreme bold, no thin weights
- Use 8px border-radius for interactive elements, and arched 16px radii for larger cards
- Trust whitespace as a courtyard — never fill available space just because it's empty
- Keep all transitions at 0.4s ease-in-out — consistency in motion matches the unhurried warmth
- Use warm, sunlit imagery on plaster-white backgrounds for showcases
- Center CTAs horizontally below section titles — the vertical rhythm is headline → subtitle → buttons
- Maintain the Serif/Sans split — serif for hero headlines, sans-serif for everything functional

### Don't
- Add drop shadows to any element — elevation through shadow contradicts the flat, sun-baked aesthetic
- Use more than three chromatic accents beyond terracotta — the palette is intentionally earth-toned
- Apply gradients, neon colors, or cool grays — the palette must remain warm and sun-faded
- Use text larger than 42px on the web — the typography is deliberately restrained even at hero scale
- Add heavy borders to cards or containers — separation is achieved through spacing and subtle clay lines
- Use uppercase text transforms — the style's warmth is expressed through lowercase calm
- Introduce sharp 90° corners or tiny 2px radii — the 8px+ radius and arch motif are deliberate
- Override the warm serif/sans pairing with cold or overly modern typefaces
- Add hover animations with scale/translate transforms — interactions are color-only (background and border transitions)
- Clutter the viewport with multiple CTAs — every screen should have at most two action buttons

## 8. Responsive Behavior

### Breakpoints
| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | <768px | Single-column layout, hamburger nav replaces horizontal labels, hero text scales to ~30px, CTA buttons stack vertically, category cards become full-width |
| Tablet | 768-1024px | 2-column nav panel, hero maintains full-viewport height, CTAs remain side-by-side, reduced horizontal padding |
| Desktop | 1024-1440px | Full horizontal nav, 3-column experience grid in dropdown, hero at 42px, side-by-side CTAs at 220px/180px width |
| Large Desktop | >1440px | Content remains centered, hero photography scales to fill wider viewports, max-width container for nav panel content |

### Touch Targets
- Primary CTA buttons: 220px × 44px minimum (well above 44×44px WCAG requirement)
- Nav buttons: minimum 36px height with 6px 16px padding — adequate touch targets
- Carousel arrows: ~48px square warm semi-transparent buttons at viewport edges
- Text links ("Explore", "Reserve"): 14px text with adequate line-height spacing for touch

### Collapsing Strategy
- **Navigation**: Horizontal category buttons (Explore, History, Visit, Events, Shop) collapse to a hamburger/drawer menu on mobile
- **Hero CTA pair**: Side-by-side buttons on desktop stack vertically on mobile
- **Category cards**: 2-up horizontal layout collapses to single-column full-width on mobile
- **Experience grid**: 3-column grid in desktop nav panel becomes 2-column on tablet, single-column on mobile
- **Spacing**: Section vertical padding remains generous (viewport-height sections) but horizontal padding reduces

### Image Behavior
- Hero images are fully responsive and fill the entire viewport at every breakpoint
- Mission carousel images use `object-fit: cover` to maintain warm composition across widths
- Experience images in the nav panel scale proportionally within their grid cells
- Category card images maintain their landscape ratio and clip via `overflow: hidden` with arched border-radius

## 9. Agent Prompt Guide

### Quick Color Reference
- Primary CTA: "Terracotta (#C25E3D)"
- Background: "Plaster White (#F7F4EF)"
- Heading text: "Mission Brown (#5C4033)"
- Body text: "Adobe Graphite (#4A4540)"
- Tertiary text: "Wrought Iron (#6E665F)"
- Placeholder: "Dust Gray (#A8A199)"
- Alternate surface: "Adobe Sand (#E8E0D5)"
- Dark surface: "Mission Brown (#5C4033)"
- Accent blue: "Cobalt (#1E4D8C)"
- Accent green: "Sage (#7A8B6E)"
- Accent gold: "Golden Ochre (#D4A35A)"

### Example Component Prompts
- "Create a hero section with a full-viewport warm mission courtyard background, centered 'San Miguel Mission' title in a warm serif at 42px weight 600 in Plaster White, a subtitle line below, and two buttons side by side: a primary Terracotta (#C25E3D) 'Plan a Visit' button and a secondary white 'View Events' button, both with 8px border-radius and 44px height"
- "Design a navigation bar with a simple mission bell or cross icon on the left, five text buttons (14px, weight 600, Mission Brown #5C4033) centered, and three icon buttons on the right, all on a warm white background with no heavy shadow"
- "Build an experience card grid with 3 columns, each card showing a warm mission image above an experience name (18px, weight 600, Mission Brown) and two text links (14px, weight 400, Wrought Iron #6E665F) labeled 'Explore' and 'Reserve', on a Plaster White surface with subtle Clay Borders"
- "Create a category card with full-bleed mission photography, arched top corners (16px) and rounded bottom corners (12px), overflow hidden, and a warm text label ('Courtyards') positioned in the top-left corner with no overlay gradient"
- "Design a persistent bottom bar with a concierge input ('What would you like to explore?' placeholder), a send icon, and a secondary CTA ('View Upcoming Events') with a Golden Ochre icon, anchored to the viewport bottom on a Plaster White background"

### Iteration Guide
When refining existing screens generated with this design system:
1. Focus on ONE component at a time — the system's warmth comes from careful detail, so each element must feel hand-finished
2. Reference specific color names and hex codes from this document — the palette is intentionally small and warm
3. Use natural language descriptions, not CSS values — "arched doorway corners" not "border-radius: 16px"
4. Describe the desired "feel" alongside specific measurements — "courtyard-like openness between sections" communicates the whitespace philosophy better than "margin-bottom: 100vh"
5. Always verify that photography and texture are doing the emotional heavy-lifting — if the UI feels cold or corporate, it's too much
