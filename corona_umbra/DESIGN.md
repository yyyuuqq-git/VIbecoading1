---
name: Corona & Umbra
colors:
  surface: '#131317'
  surface-dim: '#131317'
  surface-bright: '#39393d'
  surface-container-lowest: '#0e0e12'
  surface-container-low: '#1b1b1f'
  surface-container: '#1f1f23'
  surface-container-high: '#2a292e'
  surface-container-highest: '#353439'
  on-surface: '#e5e1e7'
  on-surface-variant: '#d0c6ab'
  inverse-surface: '#e5e1e7'
  inverse-on-surface: '#303034'
  outline: '#999077'
  outline-variant: '#4d4732'
  surface-tint: '#e9c400'
  primary: '#fff6df'
  on-primary: '#3a3000'
  primary-container: '#ffd700'
  on-primary-container: '#705e00'
  inverse-primary: '#705d00'
  secondary: '#ddb7ff'
  on-secondary: '#4a0080'
  secondary-container: '#622599'
  on-secondary-container: '#d1a1ff'
  tertiary: '#f7f6f6'
  on-tertiary: '#2f3131'
  tertiary-container: '#dadada'
  on-tertiary-container: '#5e5f5f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe16d'
  primary-fixed-dim: '#e9c400'
  on-primary-fixed: '#221b00'
  on-primary-fixed-variant: '#544600'
  secondary-fixed: '#f0dbff'
  secondary-fixed-dim: '#ddb7ff'
  on-secondary-fixed: '#2c0050'
  on-secondary-fixed-variant: '#622599'
  tertiary-fixed: '#e3e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#464747'
  background: '#131317'
  on-background: '#e5e1e7'
  surface-variant: '#353439'
typography:
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 36px
    fontWeight: '600'
    lineHeight: 44px
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 40px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Space Mono
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
---

## Brand & Style
The design system is built around the celestial awe of a total solar eclipse—the precise moment where shadow meets light. It targets an audience seeking a transformative, energetic festival experience. 

The design style is **Glassmorphism meets High-Contrast Bold**. It utilizes deep, "infinite" space blacks as a canvas, punctuated by radiant, glowing "corona" effects. Translucent layers mimic atmospheric haze, while sharp, brilliant highlights represent the "diamond ring" effect. The aesthetic is cosmic, mysterious, and high-energy, evoking the visceral feeling of standing under a darkened sun.

## Colors
The palette is rooted in the transition from totality to enlightenment.

- **Primary (Sun-Gold):** `#FFD700`. Used for the most critical actions and to represent the solar corona. It should glow with a subtle outer bloom.
- **Secondary (Deep Indigo):** `#4B0082`. Used for background gradients, depth, and atmospheric layering.
- **Tertiary (Moon-Gray):** `#C0C0C0`. A metallic, cool neutral used for secondary text and structural borders.
- **Base (Space Black):** `#050508`. A near-perfect black to ensure maximum contrast for glowing elements.

Functional colors like success and error should be shifted toward the celestial theme: a "Nebula Green" and a "Supernova Red."

## Typography
The typography strategy contrasts technical precision with monumental scale. 

**Space Grotesk** is used for headlines to provide a futuristic, geometric edge. Large display sizes should use tight tracking to feel more impactful. **Hanken Grotesk** provides a highly legible, clean sans-serif experience for information-heavy sections, maintaining a modern and professional tone. **Space Mono** is reserved for metadata, timestamps, and "technical" festival data, grounding the cosmic theme with a sense of astronomical data tracking.

## Layout & Spacing
The layout follows a **Fluid Grid** model with generous vertical breathing room to simulate the vastness of space.

- **Grid:** A 12-column system for desktop, 4-column for mobile.
- **Rhythm:** Use an 8px base unit. Section spacing should be aggressive (e.g., 120px or 160px) to allow hero elements to "float" without crowding.
- **Safe Areas:** Maintain wide margins on desktop (64px+) to keep content centered and focused, mimicking the ocular view of a telescope.

## Elevation & Depth
Depth is created through **Glassmorphism and Tonal Gradients** rather than traditional shadows.

- **Surfaces:** UI containers use a semi-transparent Deep Indigo background (`rgba(75, 0, 130, 0.2)`) with a high-intensity `backdrop-filter: blur(20px)`.
- **Borders:** Instead of heavy shadows, use 1px "Ghost Borders." These are linear gradients that transition from semi-transparent white (top-left) to transparent (bottom-right) to catch the "light" of the corona.
- **Glows:** Higher elevation elements (like active modals) should have an outer `box-shadow` using the Sun-Gold color with a very large blur radius (40px+) and low opacity (0.3) to simulate a light bleed.

## Shapes
The shape language is primarily **Rounded**, reflecting the orbital and spherical nature of the sun and moon. 

Standard components use a 0.5rem radius, while interactive buttons and decorative chips often use pill-shapes (3) to suggest motion and fluidity. Avoid sharp 0px corners, as they feel too aggressive for the naturalistic, celestial theme.

## Components
- **Buttons:** Primary buttons are Sun-Gold with black text, utilizing a "Pulse" hover effect. Secondary buttons are ghost-style with Sun-Gold borders.
- **Cards:** Use the glassmorphic style—deep indigo tint, backdrop blur, and a subtle 1px top-edge highlight.
- **Inputs:** Dark backgrounds with a 1px Moon-Gray bottom border. On focus, the border transitions to a Sun-Gold gradient.
- **Chips/Tags:** Monospaced text inside pill-shaped, semi-transparent indigo containers.
- **Countdown Timers:** A custom component using large Space Grotesk weights, essential for the "minutes to totality" festival feature.
- **Navigation:** A floating, blurred-glass dock at the bottom of the screen on mobile, and a minimal top-aligned transparent bar on desktop.