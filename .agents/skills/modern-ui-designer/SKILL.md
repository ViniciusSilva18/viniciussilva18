---
name: modern-ui-designer
description: >-
  Specialized skill for creating stunning, eye-catching, and modern UI/UX
  designs inspired by high-end design libraries (Bento grids, Glassmorphism,
  neon dark modes, smooth micro-animations, and rich typography).
---

# Modern UI Designer (High-End & Prompts Library Standard)

Guarantees that every frontend application, dashboard, or landing page looks like a top-tier digital product crafted by a senior product designer, avoiding generic AI templates.

## Core Design Principles

### 1. Color System & Palettes
- **Dark Elegance**: Deep background foundations (`#090d16`, `#0f172a`, `#111827`) instead of flat black `#000000`.
- **Harmonious Accents**: Vibrant gradients using HSL tailored colors (e.g., Emerald `#10b981` to Cyan `#06b6d4`, or Violet `#8b5cf6` to Fuchsia `#d946ef`).
- **Surface Elevation**: Layer cards with subtle borders (`1px solid rgba(255, 255, 255, 0.08)`) and soft radial glow highlights.

### 2. Glassmorphism & Depth
- Use `backdrop-filter: blur(16px)` with semi-transparent background fills (`rgba(17, 24, 39, 0.7)`).
- Multi-layered box shadows (`box-shadow: 0 10px 30px -10px rgba(0, 0, 0, 0.5)`).

### 3. Typography Hierarchy
- Import Google Fonts (*Inter*, *Plus Jakarta Sans*, *Outfit*, or *Space Grotesk*).
- Never use default browser fonts (e.g. Times New Roman, standard Arial).
- Use distinct font weights (`400` body, `600` subheadings, `800` titles) with tight letter-spacing on large headings (`letter-spacing: -0.02em`).

### 4. Interactive Micro-Animations & Bento Grids
- **Bento Grid Layouts**: Asymmetrical grids where featured items take `col-span-2` or `row-span-2`.
- **Micro-interactions**: Smooth hover transitions (`transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1)`), subtle scale lifts (`transform: translateY(-4px)`), and glowing borders.
- **Dynamic Feedback**: Skeleton loaders, animated pulsing indicators, and interactive toast notifications.
