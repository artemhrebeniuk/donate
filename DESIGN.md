---
name: Ethereal Glass
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1b1b1d'
  surface-container: '#1f1f21'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#303032'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#ffb3ae'
  on-secondary: '#68000b'
  secondary-container: '#940b19'
  on-secondary-container: '#ff9e98'
  tertiary: '#ffffff'
  on-tertiary: '#003828'
  tertiary-container: '#88f7cc'
  on-tertiary-container: '#007355'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#ffdad7'
  secondary-fixed-dim: '#ffb3ae'
  on-secondary-fixed: '#410004'
  on-secondary-fixed-variant: '#910717'
  tertiary-fixed: '#88f7cc'
  tertiary-fixed-dim: '#6bdbb1'
  on-tertiary-fixed: '#002116'
  on-tertiary-fixed-variant: '#00513b'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 17px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: -0.001em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.05em
  button-text:
    fontFamily: Inter
    fontSize: 15px
    fontWeight: '600'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  xs: 4px
  base: 8px
  sm: 12px
  md: 24px
  gutter: 24px
  margin: 32px
  lg: 48px
  xl: 80px
---

## Brand & Style
The brand personality is a sophisticated fusion of **Glassmorphism** and **Minimalism**. It aims to evoke a sense of futuristic reliability and premium transparency. The target audience consists of tech-savvy individuals and developers who appreciate high-end visual polish and "low-friction" interactions.

The visual style is characterized by deep, atmospheric backgrounds punctuated by vibrant, blurred orbital elements (bubbles) that create depth without physical shadows. The interface feels "airy" despite the dark mode, utilizing light as a structural material through semi-transparent surfaces and soft glowing borders.

## Colors
The palette is rooted in a deep, multi-tonal dark theme. The background is a subtle diagonal gradient from pure black to a muted midnight violet. 

- **Primary:** Pure white, used for high-impact text and high-contrast primary actions.
- **Semantic Accents:** Specific brand colors are used for external platform recognition (Mono-black, Ko-fi Red, Crypto Green).
- **Glass System:** Transparency is the core medium. Surfaces use a very low-opacity white fill with a slightly more opaque white border to define edges against the dark background.

## Typography
The system uses **Inter** exclusively to maintain a utilitarian, Swiss-inspired clarity that balances the decorative glass effects. 

- **Hierarchy:** Dramatic contrast between the 48px Display Bold and the 17px Body Text creates a clear entry point.
- **Refinement:** Tight letter-spacing on headlines ensures they feel "designed" and modern, while expanded tracking on label-caps ensures readability at small sizes.
- **Coloration:** Body text uses a secondary "on-surface-variant" (muted grey) to reduce visual noise compared to pure white headings.

## Layout & Spacing
The layout follows a **Fixed Grid** approach for the main content canvas, centered horizontally with a max-width of 980px to maintain focus on the donation options.

- **Grid:** A 3-column responsive grid is used for desktop, collapsing to 1-column on mobile.
- **Rhythm:** An 8px base unit drives the spacing scale. Large vertical gaps (80px) are used between sections to allow the background "bubbles" to breathe.
- **Paddings:** Internal card padding is set to 24px (md), creating a generous touch target and breathing room for icons and text.

## Elevation & Depth
Elevation is achieved through **Glassmorphism** and **Luminous Shadows** rather than standard black dropshadows.

- **Stacking:** Elements use `backdrop-filter: blur(20px)` to pull color from the background bubbles while remaining distinct.
- **Glows:** High-priority elements (like the Logo and Action Buttons) utilize semi-transparent white or colored outer glows (`box-shadow`) to simulate a light source emitting from the element itself.
- **Borders:** "Ghost borders" (1px white/10%) are essential to define the silhouette of surfaces against the dark background.

## Shapes
The shape language is primarily **Rounded**, favoring 12px to 16px corners for cards and buttons to soften the tech-heavy aesthetic. 

- **Cards:** Use `rounded-xl` (12px-16px) for a modern, friendly feel.
- **Interactive Elements:** Buttons use a slightly tighter `rounded-lg` (8px-10px) to distinguish them from the containers they sit in.
- **Avatars/Icons:** Circles are used for logos and icon backgrounds to create a sense of harmony with the background "bubbles."

## Components
- **Buttons:** Large, high-contrast blocks. Primary buttons should use high-opacity white (90%) with black text. Secondary brand buttons use brand colors with white text. All buttons feature a subtle glow matching their background color.
- **Glass Cards:** Containers with `bg-white/5`, a thin border, and backdrop blur. Hover states should increase the background opacity to `white/10` and sharpen the border brightness.
- **Icons:** Material Symbols (Outlined) are used at a 24px scale, housed within circular backgrounds that carry a thematic color or glow.
- **Backdrop Bubbles:** Decorative, non-interactive elements using `filter: blur(20px-50px)` and low-opacity radial gradients to create atmospheric depth.
- **Selection:** Use `primary-container` (soft white/grey) for background and `on-primary-container` for text to maintain the clean aesthetic even during interaction.