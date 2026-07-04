---
name: SkyWay Terminal Directory
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f4'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#43474f'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f0f1f1'
  outline: '#737780'
  outline-variant: '#c3c6d1'
  surface-tint: '#3a5f94'
  primary: '#001e40'
  on-primary: '#ffffff'
  primary-container: '#003366'
  on-primary-container: '#799dd6'
  inverse-primary: '#a7c8ff'
  secondary: '#bb0024'
  on-secondary: '#ffffff'
  secondary-container: '#e41d35'
  on-secondary-container: '#fffbff'
  tertiary: '#1b1f21'
  on-tertiary: '#ffffff'
  tertiary-container: '#303436'
  on-tertiary-container: '#999c9e'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d5e3ff'
  primary-fixed-dim: '#a7c8ff'
  on-primary-fixed: '#001b3c'
  on-primary-fixed-variant: '#1f477b'
  secondary-fixed: '#ffdad8'
  secondary-fixed-dim: '#ffb3b0'
  on-secondary-fixed: '#410006'
  on-secondary-fixed-variant: '#93001a'
  tertiary-fixed: '#e0e3e5'
  tertiary-fixed-dim: '#c4c7c9'
  on-tertiary-fixed: '#191c1e'
  on-tertiary-fixed-variant: '#444749'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  terminal-number:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  terminal-number-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '800'
    lineHeight: 40px
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Hanken Grotesk
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
  airline-code:
    fontFamily: JetBrains Mono
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 24px
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  grid-margin: 2rem
  grid-gutter: 1.5rem
  section-gap: 4rem
  card-padding: 1.25rem
  terminal-row-gap: 2rem
---

## Brand & Style

The design system is engineered for the high-stakes, fast-moving environment of an international airport terminal. It adopts a **Corporate / Modern** aesthetic with a premium finish, echoing the reliability and precision of aviation. 

The personality is authoritative yet welcoming, using the iconic palette of a major carrier to instill immediate trust. The UI utilizes a structured, information-first approach—minimizing cognitive load for travelers while maintaining a sophisticated, high-end feel. Key visual motifs include subtle metallic gradients, crisp geometric boundaries, and a "flight-deck" clarity that prioritizes legibility above all else.

## Colors

This design system utilizes a palette rooted in deep maritime blues and striking reds. 

- **Primary (Navy Blue):** Used for navigation bars, terminal headers, and primary buttons. It represents stability and professional excellence.
- **Secondary (Red):** Reserved for accentuation, call-to-actions, and critical alerts. It serves as a visual "north star" in a sea of data.
- **Tertiary (Cloud Silver):** Used for borders, dividers, and secondary iconography to provide a sophisticated, metallic touch.
- **Neutral (White/Slate):** Large surface areas use clean white to maximize readability under harsh airport lighting, with slate grays used for secondary body text.

## Typography

Typography is the backbone of the directory. We use **Hanken Grotesk** for display and terminal headers to provide a sharp, contemporary look that feels engineered and precise. 

**Inter** is the workhorse for body content, chosen for its exceptional legibility at small sizes and high x-height. For airline codes and technical data (gates, times), **JetBrains Mono** is employed to give a clear, monospaced "flight manifest" feel, ensuring that characters like 'I' and '1' are never confused.

## Layout & Spacing

The layout follows a **Fixed Grid** model on desktop to mirror the structured environment of an airport display. 

- **Desktop:** 12-column grid with a max-width of 1280px. Terminal sections are grouped in high-contrast blocks.
- **Tablet:** 8-column grid. Information cards reflow into two-column layouts.
- **Mobile:** Single column. Margins are reduced to 16px to maximize content area for airline codes.

Spacing is generous between terminal sections to prevent visual bleed. Within sections, airline code cards are packed tightly but rhythmically to allow for quick scanning of alphabetical lists.

## Elevation & Depth

To maintain a premium, architectural feel, the design system uses **Tonal Layers** combined with **Low-contrast outlines**. 

- **Level 0 (Background):** Solid off-white or light gray surface.
- **Level 1 (Section Containers):** White surfaces with a 1px solid border in Cloud Silver.
- **Level 2 (Active Cards):** A very soft, 12% opacity Navy Blue shadow is used only when a terminal or airline is "selected" or "active."

Shadows are avoided on static elements to keep the UI feeling like a physical signage system rather than a floating web app. Depth is primarily communicated through color-blocking (Navy headers vs. White content areas).

## Shapes

The shape language is **Soft (0.25rem)**. This subtle rounding provides a modern touch without sacrificing the professional, "square-jawed" look of an enterprise system. 

Airline code cards utilize the standard `rounded-sm` for a crisp look, while large terminal-level containers may use `rounded-lg` (0.5rem) to differentiate them as primary structural elements. Buttons and search fields follow the 0.25rem standard to maintain consistency with the airline's brand identity guidelines.

## Components

### Airline Code Cards
Individual tiles featuring the two-letter IATA code in **JetBrains Mono**. These should have a subtle Cloud Silver border. When an airline is a "Frequently Seen" carrier (marked with *), the card gains a small Red corner-accent or a secondary label.

### Terminal Headers
Full-width Navy Blue bars. The terminal number should be prominently displayed on the left in white Hanken Grotesk. The right side is reserved for quick-links like "Gate Map" or "Ground Transport."

### Search & Filter
A persistent, high-contrast input field with a prominent magnifying glass icon. On mobile, this sticks to the top of the viewport to allow travelers to find their airline instantly.

### Status Chips
Small, high-visibility badges used within airline lists to denote "Partner Flight," "Codeshare," or "Terminal Transfer Required." These use the `label-caps` typography style.

### Directional Lists
Lists for terminal services (Dining, Lounges) should use high-contrast iconography and chevron indicators to suggest movement and direction.