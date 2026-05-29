---
name: Syntactic Flux
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c2c6d6'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8c909f'
  outline-variant: '#424754'
  surface-tint: '#adc6ff'
  primary: '#adc6ff'
  on-primary: '#002e6a'
  primary-container: '#4d8eff'
  on-primary-container: '#00285d'
  inverse-primary: '#005ac2'
  secondary: '#d0bcff'
  on-secondary: '#3c0091'
  secondary-container: '#571bc1'
  on-secondary-container: '#c4abff'
  tertiary: '#4edea3'
  on-tertiary: '#003824'
  tertiary-container: '#00a572'
  on-tertiary-container: '#00311f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#e9ddff'
  secondary-fixed-dim: '#d0bcff'
  on-secondary-fixed: '#23005c'
  on-secondary-fixed-variant: '#5516be'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
typography:
  headline-lg:
    fontFamily: Geist
    fontSize: 30px
    fontWeight: '600'
    lineHeight: 36px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  headline-sm:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  code-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  code-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 18px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 24px
  panel-sidebar: 260px
---

## Brand & Style

The design system is engineered for developers and technical architects, prioritizing speed of comprehension and structural clarity. The brand personality is precise, technical, and high-performance, evoking the feel of a premium, high-end IDE integrated into a modern SaaS environment.

The visual style is **Corporate / Modern** with a **Technical** edge. It utilizes a deep slate palette to minimize eye strain during long periods of code review and migration orchestration. The interface relies on crisp borders and intentional spacing to manage high data density without creating visual clutter. The emotional response should be one of control and reliability—tools that work as hard and as accurately as the developers using them.

## Colors

The palette is optimized for a dark-first experience. 
- **Primary (Blue):** Reserved for core actions, progress indicators, and primary navigation states.
- **Secondary/AI (Violet):** Specifically used for LLM-powered features, automated suggestions, and migration "magic" moments.
- **Background & Surface:** A tiered system of deep slates (`#0F172A` for the canvas and `#1E293B` for panels/cards) creates a clear hierarchy of information.
- **Semantic Colors:** Emerald for successful migrations/passed checks; Amber for warnings or linting errors.

Contrast ratios must adhere strictly to WCAG AA standards for legibility against the deep background.

## Typography

This design system uses a three-font architecture:
1. **Geist:** Used for headlines and page titles to provide a clean, technical, and modern aesthetic.
2. **Inter:** The workhorse for UI elements, labels, and standard body text, chosen for its exceptional readability at small sizes.
3. **JetBrains Mono:** Dedicated to code blocks, AST tree nodes, and technical metadata.

Typography scales are compact to allow for maximum information density. On mobile, `headline-lg` should scale down to `24px` to prevent excessive wrapping.

## Layout & Spacing

The layout follows a **Fluid Grid** model with fixed-width utility panels (sidebars and inspectors). 
- **System Grid:** A 12-column system is used for dashboard layouts, while code-heavy views use a flexible split-pane model.
- **Rhythm:** An 8px-based spacing system is standard, with a 4px "half-step" used for tight component internals (e.g., button icons, list items).
- **Density:** High-density spacing is preferred. Margins between logical sections should be `24px` on desktop, while internal component padding should remain tight (`8px` to `12px`).
- **Breakpoints:** 
  - Mobile: < 768px (Single column, hidden sidebars)
  - Tablet: 768px - 1280px (Collapsible sidebars)
  - Desktop: > 1280px (Permanent navigation, multi-pane views)

## Elevation & Depth

Hierarchy is established through **Tonal Layers** and **Low-Contrast Outlines** rather than heavy shadows.
- **Level 0 (Background):** `#0F172A` — The base canvas.
- **Level 1 (Surface):** `#1E293B` — Used for primary content areas, cards, and sidebars.
- **Level 2 (Overlay):** `#334155` — Used for modals, tooltips, and floating menus.

Each elevated element should have a subtle 1px border using `#334155` or `#475569` to define its edge. Ambient shadows are only used for global overlays (modals), utilizing a deep, 20% opacity black with a 12px blur and no offset.

## Shapes

The design system uses a **Soft** shape language to maintain a professional, technical feel while appearing modern.
- Standard components (Buttons, Inputs, Chips) use a `4px` (0.25rem) radius.
- Larger containers (Cards, Modals) use an `8px` (0.5rem) radius.
- Progress bars and status dots may use "full" rounding (pill-shaped) to distinguish them from structural UI elements.

## Components

- **Buttons:** Primary buttons use a solid `#3B82F6` fill with white text. AI-action buttons use a gradient or solid `#8B5CF6`. Ghost buttons are preferred for secondary actions to keep the UI clean.
- **Input Fields:** Dark backgrounds (`#0F172A`) with a 1px slate border. Focus states must use a 2px `#3B82F6` ring.
- **Chips/Badges:** Small, tight padding (2px top/bottom, 8px left/right). Use subdued background tints of semantic colors (e.g., Emerald at 10% opacity) with high-contrast text.
- **Lists & Tables:** Row heights should be compact (32px-40px). Use subtle divider lines (`#334155`) rather than alternating row colors.
- **Code Blocks:** Syntax highlighting should be based on the "Nord" or "One Dark" themes. Line numbers are mandatory. Diff views use full-width green/red background tints at 15% opacity.
- **AST Tree:** Use line-based connectors and `JetBrains Mono` at `12px`.
- **Status Indicators:** Use a combination of a colored dot and text label for accessibility.