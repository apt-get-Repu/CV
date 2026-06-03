---
name: Modern Archive
colors:
  surface: '#fcf9ee'
  surface-dim: '#dddad0'
  surface-bright: '#fcf9ee'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f7f4e9'
  surface-container: '#f1eee3'
  surface-container-high: '#ebe8dd'
  surface-container-highest: '#e5e3d8'
  on-surface: '#1c1c15'
  on-surface-variant: '#4c4546'
  inverse-surface: '#31312a'
  inverse-on-surface: '#f4f1e6'
  outline: '#747878'
  outline-variant: '#cfc4c5'
  surface-tint: '#5e5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1b1b1b'
  on-primary-container: '#848484'
  inverse-primary: '#c6c6c6'
  secondary: '#5c614c'
  on-secondary: '#ffffff'
  secondary-container: '#e0e5ca'
  on-secondary-container: '#626751'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#2c1600'
  on-tertiary-container: '#a57c52'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#e0e5ca'
  secondary-fixed-dim: '#c4c9af'
  on-secondary-fixed: '#191d0d'
  on-secondary-fixed-variant: '#444935'
  tertiary-fixed: '#ffdcbd'
  tertiary-fixed-dim: '#edbe8e'
  on-tertiary-fixed: '#2c1600'
  on-tertiary-fixed-variant: '#61401b'
  background: '#fcf9ee'
  on-background: '#1c1c16'
  surface-variant: '#e5e3d8'
  paper-overlay: rgba(255, 255, 255, 0.03)
typography:
  display-lg:
    fontFamily: Bodoni Moda
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Bodoni Moda
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Bodoni Moda
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Bodoni Moda
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  quote:
    fontFamily: Bodoni Moda
    fontSize: 22px
    fontWeight: '400'
    lineHeight: '1.5'
  body-lg:
    fontFamily: Source Sans Three
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Source Sans Three
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Source Sans Three
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
spacing:
  container-max: 1140px
  section-gap: 80px
  unit: 8px
  gutter: 24px
  margin-mobile: 20px
---

## Brand & Style

The brand identity is rooted in the "Archive" aesthetic—a sophisticated blend of classical editorial design and modern digital precision. It targets an intellectual audience that values rigor, history, and clarity. 

The visual style is **Minimalist-Editorial**. It leverages heavy whitespace, high-contrast serif typography, and a "paper-like" tactile quality to evoke the feeling of a prestige journal or a curated museum exhibition. The emotional response is one of authority, silence, and timelessness. The design rejects modern trends like rounded corners and vibrant gradients in favor of sharp edges, a monochromatic foundation, and subtle textures (like the paper grain overlay) that suggest physical permanence.

## Colors

The palette is anchored by a warm, bone-colored neutral (`#fcf9ee`) that serves as the "paper" substrate. This prevents the harshness of pure white and establishes an archival feel. 

- **Primary:** Pure black (`#000000`) is used for core structural elements, borders, and high-emphasis text.
- **Secondary:** A muted, scholarly olive (`#5c614c`) used for subtle accents and date indicators.
- **Tertiary:** A refined tobacco-tan (`#a57c52`) reserved for decorative highlights and specialized labels.
- **Neutral:** A range of parchment-inspired tones used for container backgrounds to create hierarchy without relying on shadows.

In Dark Mode, the palette inverts to deep charcoals and warm grays, maintaining the "ink on paper" contrast ratio while reducing eye strain.

## Typography

The typographic system is a dialogue between two extremes:
1. **The Humanist Serif (Bodoni Moda):** Used for headlines and quotes. Its high contrast between thick and thin strokes provides the editorial authority. It should frequently be used in italics for professional titles and pull quotes.
2. **The Modernist Sans (Source Sans Three):** Used for body copy and metadata. It provides a functional, neutral counterpoint that ensures legibility in dense information blocks.

**Key Rule:** Large-scale headings (`display-lg`) should always use tight tracking and leading. Small labels (`label-caps`) should use expanded tracking to maximize readability at tiny scales.

## Elevation & Depth

This system avoids ambient shadows entirely, opting for **Tonal Layers** and **Bold Outlines**.

- **Depth via Tone:** Surfaces are layered using slightly different neutral shades (e.g., `surface-container-low` for secondary sections) to suggest hierarchy.
- **Structural Lines:** Hierarchy is defined by 1px borders and "double dividers" (a 2px top border and 1px bottom border). This mimics the layout of a traditional newspaper or ledger.
- **Micro-Textures:** A persistent 3% white noise overlay (`paper-overlay`) sits above the background to give the UI a tactile, non-digital quality.
- **Interactive States:** Hover effects are indicated by a full-color reveal of grayscale images or a solid background color fill, rather than an elevation lift.

## Shapes

The shape language is strictly **Sharp (0px)**. 

Every UI element—from buttons and input fields to project cards and imagery—must have 90-degree corners. This reinforces the architectural and archival nature of the brand. The only circular elements permitted are micro-icons or bullet points used as structural markers in lists. 

Large imagery should be treated as "plates" in a book, often featuring thin borders to separate them from the background.

## Components

- **Buttons:** Outlined by default with a 1px border. On hover, they perform a sharp inversion (background fills with text color). No rounded corners.
- **Dividers:** Use a "Double Divider" for primary section transitions—two parallel lines of varying weights (2px and 1px) separated by 2px of space.
- **Input Fields:** Minimalist "ghost" inputs. No bounding box; only a 1px bottom border that changes color on focus.
- **Cards:** Defined by their content and a subtle background tint (`surface-container`). They do not use shadows.
- **Images:** Always rendered in grayscale by default, transitioning to color only on user interaction (hover). This maintains the monochromatic aesthetic of the "archive" until the user actively explores a project.
- **Section Titles:** Accompanied by a small "Sección [X]" label in `label-caps` and a 60px wide underline (1px height) to anchor the start of a narrative.