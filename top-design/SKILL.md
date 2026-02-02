---
name: top-design
description: >
  Create award-winning websites and applications with design and typography rated 10/10.
  Use this skill when building premium digital experiences that match the quality of elite
  agencies like Locomotive, Studio Freight, AREA 17, Active Theory, Hello Monday, Dogstudio,
  Tonik, Instrument, Resn, and Awwwards winners. Triggers include premium design, award-winning,
  agency-level, Awwwards quality, exceptional typography, immersive experience, 10/10 design,
  portfolio site, brand website, creative agency style, top-tier web design, or when building
  sites for luxury brands, tech companies, cultural institutions, or startups requiring
  exceptional visual craft.
license: MIT
metadata:
  author: wondelai
  version: "1.0"
---

# Top-Design: Award-Winning Digital Experiences

Create websites and applications at the level of world-class digital agencies. This skill embodies the craft of studios that consistently win FWA, Awwwards, CSS Design Awards, and Webby Awards.

## Core Philosophy

**The agencies you're emulating share these traits:**
- Every pixel is intentional — nothing default, nothing accidental
- Typography IS the design — not decoration, but architecture
- Motion creates emotion — animation serves narrative, not novelty
- White space is a weapon — tension through restraint
- Performance is non-negotiable — 60fps or nothing

**What separates 10/10 from 8/10:**
- 8/10: Good typography, nice colors, smooth animations
- 10/10: Typography that makes you gasp, colors that feel invented, animations that tell stories

## Design Process

### 1. Concept First, Code Second

Before any code, define:

```
BRAND ESSENCE: What single word captures the soul?
VISUAL TENSION: What opposing forces create interest?
SIGNATURE MOMENT: What will people screenshot and share?
TECHNICAL AMBITION: What pushes the browser's limits?
```

### 2. Typography as Architecture

**Font Selection Hierarchy:**

```
DISPLAY/HERO: The statement maker
├── Custom/Variable fonts (preferred)
├── Foundry fonts: Pangram Pangram, Dinamo, Grilli Type, Klim, Commercial Type
├── Premium Google: Space Grotesk, Instrument Serif, Fraunces
└── NEVER: Inter, Roboto, Arial, system-ui

BODY: The workhorse
├── Match personality to display font
├── Legibility at 16-18px minimum
└── Consider: Söhne, GT America, Suisse, Neue Montreal
```

**Typography Principles:**
- Massive scale contrast: 200px hero + 14px body
- Negative tracking on large type (-0.02em to -0.05em)
- Generous line-height for body (1.5-1.7)
- Tight line-height for display (0.9-1.1)
- Optical alignment over mathematical alignment

### 3. Color Philosophy

**Approach Types:**

```
MONOCHROMATIC TENSION
├── 95% one dominant color/neutral
├── 5% accent that POPS
└── Example: Locomotive (cream + black + orange spark)

BOLD SIGNATURE
├── Own a color combination
├── Make it unmistakable
└── Example: Studio Freight (black + cream + rust)

CONTEXTUAL SHIFTING
├── Color responds to content
├── Sections have distinct palettes
└── Example: AREA 17 (adapts to each client case study)
```

**Technical Implementation:**
```css
:root {
  /* Never just 'black' or 'white' */
  --color-dark: #0a0a0a;
  --color-light: #fafaf9;
  --color-accent: #ff4d00;
  
  /* Functional hierarchy */
  --color-text-primary: var(--color-dark);
  --color-text-secondary: rgba(10, 10, 10, 0.6);
  --color-surface: var(--color-light);
  --color-border: rgba(10, 10, 10, 0.1);
}
```

### 4. Layout Principles

**Grid Breaking is the Goal:**
- Start with grid, then strategically violate it
- Elements that bleed, overlap, or extend create tension
- Asymmetry > Symmetry (but with intention)

**Scroll-Based Composition:**
```
VERTICAL RHYTHM
├── Sections breathe (min 100vh for key moments)
├── Density varies (packed grids vs. single elements)
├── Reading pace controlled through spacing
└── Surprise through unexpected scale shifts
```

### 5. Animation Philosophy

**The Three Laws of Elite Motion:**

1. **Purpose Over Decoration**: Every animation answers "Why does this move?"
2. **Custom Curves, Never Linear**: Use exponential/quart easing
3. **Orchestration Over Isolation**: Elements animate in relationship

## Reference Files

Consult these for detailed implementation:

- **[references/typography.md](references/typography.md)**: Font pairing strategies, type scale systems, advanced CSS typography
- **[references/animation-patterns.md](references/animation-patterns.md)**: Scroll animations, page transitions, micro-interactions with code
- **[references/layout-systems.md](references/layout-systems.md)**: Grid frameworks, breakpoints, responsive patterns
- **[references/technical-stack.md](references/technical-stack.md)**: Libraries, tools, performance optimization
- **[references/case-studies.md](references/case-studies.md)**: Agency technique breakdowns

## Quality Checklist

Before considering any design complete:

```
TYPOGRAPHY
□ Display font makes a statement
□ Scale contrast is dramatic (min 10:1 ratio)
□ Tracking adjusted for size
□ Line-height optimized per use case
□ No orphans/widows on key headlines

MOTION
□ Page load has choreographed reveal
□ Scroll feels custom (not default)
□ Hover states provide feedback
□ Transitions use custom easing
□ 60fps verified

LAYOUT
□ Grid exists but is strategically broken
□ White space creates tension
□ Hierarchy is instantly clear
□ Mobile is designed, not adapted
□ Breakpoints feel intentional

DETAILS
□ Custom cursor (if appropriate)
□ Selection colors are branded
□ Focus states are beautiful
□ Loading states are designed
□ Error/empty states crafted

PERFORMANCE
□ Fonts subset and preloaded
□ Images optimized (WebP/AVIF)
□ Animations GPU-accelerated
□ No layout shifts
□ Sub-3s load on 3G
```

## Anti-Patterns to Avoid

```
TYPOGRAPHY CRIMES
✗ System fonts as primary typeface
✗ Uniform type scale (everything similar)
✗ Default letter-spacing on headlines
✗ Line-height: 1.5 applied universally

ANIMATION SINS
✗ Linear easing anywhere
✗ Everything animated simultaneously
✗ Animations blocking interaction
✗ Parallax without purpose

LAYOUT FAILURES
✗ Center-aligned everything
✗ Equal spacing everywhere
✗ Grid followed rigidly
✗ Mobile as afterthought

GENERIC TELLS
✗ Purple/blue gradient hero sections
✗ "Hi, I'm [Name]" portfolio intros
✗ Floating cards with box-shadows
✗ Stock photography
✗ Visible lorem ipsum
```

## Implementation Notes

1. **Start with the signature moment** — the thing that defines the experience
2. **Build mobile-first** but conceptualize desktop-first
3. **Prototype animations early** — motion is not a polish step
4. **Test on real devices** — simulators lie about performance
5. **Ship with restraint** — 3 things perfect beats 10 things mediocre
