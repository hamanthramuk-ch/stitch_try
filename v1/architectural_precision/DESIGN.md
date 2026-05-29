---
name: Architectural Precision
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#5f3f3a'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#946e68'
  outline-variant: '#e9bcb5'
  surface-tint: '#c00000'
  primary: '#b70100'
  on-primary: '#ffffff'
  primary-container: '#e60000'
  on-primary-container: '#fff7f5'
  inverse-primary: '#ffb4a8'
  secondary: '#5e5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2e2e2'
  on-secondary-container: '#646464'
  tertiary: '#595a5a'
  on-tertiary: '#ffffff'
  tertiary-container: '#727272'
  on-tertiary-container: '#faf8f8'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdad4'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#930100'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c6'
  on-secondary-fixed: '#1b1b1b'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c7c6c6'
  on-tertiary-fixed: '#1b1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
  heritage-red: '#E60000'
  ink-black: '#000000'
  graphite-gray: '#767676'
  canvas-white: '#FFFFFF'
  surface-mist: '#F2F2F2'
typography:
  headline-xl:
    fontFamily: Public Sans
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Public Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Public Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Public Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-bold:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  code-snippet:
    fontFamily: monospace
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 22px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 40px
---

## Brand & Style

The design system for CodeArch AI is rooted in the principles of institutional trust, absolute precision, and architectural clarity. It translates the sophisticated heritage of global wealth management into the context of high-end AI development and technical architecture.

The visual style is **Corporate / Modern** with a lean toward **Minimalism**. It avoids unnecessary ornamentation, favoring a structured layout that prioritizes information density and clarity. The aesthetic should feel authoritative, reliable, and deliberate—mimicking the meticulous nature of both financial auditing and complex software engineering.

**Key Brand Attributes:**
- **Authoritative:** The UI carries the weight of a trusted institution.
- **Structured:** Every element is aligned to a rigorous grid, suggesting architectural integrity.
- **Sophisticated:** A restricted color palette and generous whitespace create a premium, "quiet luxury" feel for high-stakes technical environments.

## Colors

The palette is derived from the high-contrast, prestigious world of wealth management. 

- **Primary (Heritage Red):** Used with extreme intentionality. It is reserved for primary actions, critical alerts, and brand signatures. It should never dominate the screen but rather act as a precise focal point.
- **Secondary (Ink Black):** Used for typography, structural borders, and navigation backgrounds to provide a grounded, serious foundation.
- **Tertiary (Graphite Gray):** Utilized for secondary text, metadata, and iconography, ensuring a clear hierarchy that doesn't compete with primary information.
- **Neutral (Canvas White & Surface Mist):** The background strategy relies on large fields of White (#FFFFFF) accented by Surface Mist (#F2F2F2) to define container zones and logical groupings without relying on heavy shadows.

The default mode is **Light**, reflecting the clarity and transparency required in institutional platforms.

## Typography

The typography strategy pairs **Public Sans** for headlines with **Inter** for UI and body text. This combination mimics the utilitarian yet polished feel of modern institutional Swiss design.

- **Public Sans (Headlines):** Chosen for its institutional clarity and "government-grade" reliability. It provides a strong, neutral voice that feels permanent and secure.
- **Inter (Body/Labels):** Selected for its exceptional legibility in data-heavy AI environments. It handles technical strings, logs, and dense documentation with professional neutrality.

**Rules:**
- Use `headline-xl` sparingly for landing hero sections.
- `label-bold` should be used for section headers and table headers, always in uppercase with slight tracking to denote an "archival" feel.
- Technical data and AI outputs should utilize a clean monospace fallback to differentiate generated code from system UI.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy. Content is centered within a 1280px container on desktop to maintain readability and a sense of "archival" control.

- **Rhythm:** An 8px baseline grid governs all vertical and horizontal spacing.
- **Grid:** A 12-column system is used for desktop, collapsing to 4 columns on mobile. 
- **Margins:** Generous outer margins (40px on desktop) reinforce the premium feel by allowing the interface to "breathe" within a frame.

**Responsiveness:**
- **Desktop:** Large gutters (24px) and fixed containers.
- **Tablet:** Fluid grid with 24px margins.
- **Mobile:** Elements stack vertically with 16px margins; typography scales down to mobile-specific variables to ensure readability.

## Elevation & Depth

This design system eschews dramatic shadows in favor of **Tonal Layers** and **Low-Contrast Outlines**. Depth is communicated through structural layering rather than physical simulation.

- **Surface Levels:** The primary background is `canvas-white`. Secondary areas (sidebars, secondary panels) use `surface-mist`. 
- **Borders:** Instead of shadows, use 1px solid strokes in `#767676` at 20% opacity to define card boundaries and input fields.
- **Focus States:** High-contrast 2px solid black outlines are used for keyboard navigation and focus states, emphasizing clarity over "softness."
- **Elevation Exception:** Only the most critical floating elements (e.g., global search modals) may use a subtle, 15% opacity black shadow with a 20px blur and no offset to denote they sit above the application plane.

## Shapes

The shape language is **Soft (0.25rem)**. While a wealth management identity often leans toward sharp corners, a subtle rounding provides the "modern" touch necessary for a technical AI application.

- **Standard Elements:** Buttons, input fields, and tags use a 4px (0.25rem) radius.
- **Large Containers:** Cards and modals use a 8px (0.5rem) radius to feel slightly more approachable.
- **Icons:** Should be linear, using 2px stroke weights with squared-off ends to maintain the architectural theme.

## Components

- **Buttons:** 
    - *Primary:* Heritage Red background, White text. No gradient. Squared appearance with subtle 4px rounding.
    - *Secondary:* Ink Black border (1px), Black text, White background. 
- **Input Fields:** 1px Graphite Gray border. On focus, the border becomes Ink Black with a 1px inner offset.
- **Chips/Tags:** Used for AI status and metadata. Light Gray (#F2F2F2) background with Graphite Gray text. No border.
- **Cards:** White background, 1px subtle border (#767676 @ 20%). No shadow. Vertical alignment of content is strictly adhered to the 8px grid.
- **Data Tables:** High-density, 1px horizontal dividers only. Table headers use `label-bold` with Graphite Gray text.
- **Progress Bars:** Heritage Red for the "active" fill to ensure user attention is captured during AI processing tasks.