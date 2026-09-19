---
name: Structural Clarity
colors:
  surface: '#f9f9ff'
  surface-dim: '#cfdaf2'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f0f3ff'
  surface-container: '#e7eeff'
  surface-container-high: '#dee8ff'
  surface-container-highest: '#d8e3fb'
  on-surface: '#111c2d'
  on-surface-variant: '#444653'
  inverse-surface: '#263143'
  inverse-on-surface: '#ecf1ff'
  outline: '#757684'
  outline-variant: '#c5c5d5'
  surface-tint: '#3e54c1'
  primary: '#001360'
  on-primary: '#ffffff'
  primary-container: '#002395'
  on-primary-container: '#8094ff'
  inverse-primary: '#bac3ff'
  secondary: '#bb0013'
  on-secondary: '#ffffff'
  secondary-container: '#e90c1e'
  on-secondary-container: '#fffbff'
  tertiary: '#1c1f21'
  on-tertiary: '#ffffff'
  tertiary-container: '#313436'
  on-tertiary-container: '#999c9e'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dee1ff'
  primary-fixed-dim: '#bac3ff'
  on-primary-fixed: '#001159'
  on-primary-fixed-variant: '#223aa8'
  secondary-fixed: '#ffdad6'
  secondary-fixed-dim: '#ffb4ab'
  on-secondary-fixed: '#410002'
  on-secondary-fixed-variant: '#93000d'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#f9f9ff'
  on-background: '#111c2d'
  surface-variant: '#d8e3fb'
typography:
  headline-display:
    fontFamily: Montserrat
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-bold:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  caption:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  section-gap: 120px
---

## Brand & Style

This design system is built for Ets Vitro MZ, a leader in glass and construction materials. The brand personality is rooted in **precision, architectural stability, and transparency**. The target audience includes architects, real estate developers, and high-end residential clients who value technical excellence and modern aesthetics.

The visual style is **Corporate Minimalism** infused with **Glassmorphism**. It utilizes heavy whitespace to evoke the feeling of an open architectural plan, while translucent layers and frosted glass effects directly reference the company's core product. The result is a professional, high-trust digital environment that feels as clean and enduring as the glass structures the company creates.

## Colors

The palette is driven by the corporate identity's "Royal Blue" and "Vibrant Red." 
- **Royal Blue** serves as the primary anchor, used for headers, primary actions, and structural elements to signify authority.
- **Vibrant Red** is used sparingly as a high-visibility accent for specific call-to-actions or critical highlights.
- **Neutral tones** consist of cool grays and pure whites to maintain a crisp, sterile (in a professional sense) atmosphere.
- **Glass Effects**: Semi-transparent white overlays with `backdrop-filter: blur(12px)` are used to create the signature "Vitro" look, allowing high-quality project photography to bleed through the UI layers.

## Typography

The typography strategy pairs **Montserrat** for headings with **Inter** for functional text.
- **Montserrat** provides an "architectural" feel with its geometric construction and wide stance, echoing the precision of construction blueprints.
- **Inter** is utilized for body copy and UI labels due to its exceptional legibility at small sizes and neutral, systematic character.
- **Hierarchy**: Large display headings should be used over high-resolution imagery. Use `label-bold` for technical specifications and category tags to maintain a professional, data-driven look.

## Layout & Spacing

This design system employs a **Fixed Grid** model for desktop and a **Fluid Grid** for mobile devices.
- **Desktop**: A 12-column grid with a 1280px max-width. Large 120px gaps between major sections ensure the "minimalist" feel.
- **Tablet**: 8-column grid with 32px margins.
- **Mobile**: 4-column grid with 20px margins.
- **Rhythm**: All spacing follows an 8px base scale. Padding within glass components should be generous (minimum 32px) to prevent the UI from feeling cramped against the "glass" edges.

## Elevation & Depth

Visual hierarchy is achieved through a combination of **Tonal Layers** and **Glassmorphism**.
- **Surface Level 0**: Background. Usually pure white or high-quality architectural photography.
- **Surface Level 1**: Content Cards. Uses a very subtle, light gray border (1px) with a soft, diffused shadow (Blur: 20px, Opacity: 4% Black).
- **Surface Level 2 (Glass)**: Navigation bars and floating modals. These utilize `backdrop-filter: blur(16px)` with a `rgba(255, 255, 255, 0.7)` background and a 1px white "inner glow" border to simulate the edge of a glass pane.
- **Shadows**: Avoid heavy, dark shadows. Use ambient, colored-tinted shadows (using a hint of the Primary Blue) to keep the UI light and airy.

## Shapes

To maintain a balance between "industrial construction" and "modern design," we use a **Soft (Level 1)** roundedness approach.
- Standard components (inputs, small buttons) use a **4px (0.25rem)** radius, providing a professional edge that isn't too aggressive.
- Large containers and image cards use **8px (0.5rem)** to soften the overall layout.
- Circular shapes are reserved strictly for icons and status indicators.

## Components

### Buttons
- **Primary**: Solid Royal Blue with white text. High-contrast, rectangular with slight 4px rounding.
- **Secondary (Glass)**: Frosted background with a Royal Blue border and text.
- **Accent**: Vibrant Red, reserved exclusively for "Get a Quote" or "Emergency Services."

### Input Fields
- Clean, 1px border in light gray. On focus, the border transitions to Royal Blue with a subtle outer glow. Labels are positioned above the field in `label-bold` typography.

### Cards (Project/Product)
- Use "Glass" treatment for text overlays on imagery. Images should have a slight zoom effect on hover to emphasize the material quality.

### Chips & Tags
- Used for material types (e.g., "Tempered," "Laminated"). Subtle gray background with `body-md` text, 4px radius.

### Navigation
- A persistent top bar with a glass effect. Links use `label-bold` with a blue underline animation on hover to denote stability and precision.