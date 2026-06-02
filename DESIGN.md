---
version: alpha
name: Quiet Journal
description: A minimal personal writing site with restrained editorial diagrams.
colors:
  primary: "#000000"
  secondary: "#444444"
  muted: "#8A8A8A"
  line: "#DCDCDC"
  surface: "#FFFFFF"
  surfaceSoft: "#F6F6F6"
typography:
  display:
    fontFamily: Noto Sans KR
    fontSize: clamp(42px, 5.8vw, 70px)
    fontWeight: 700
    lineHeight: 1.13
    letterSpacing: 0
  body:
    fontFamily: Noto Sans KR
    fontSize: clamp(17px, 1.5vw, 19px)
    fontWeight: 400
    lineHeight: 1.92
    letterSpacing: 0
  label:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: 800
    lineHeight: 1.5
    letterSpacing: 0
spacing:
  xs: 8px
  sm: 12px
  md: 20px
  lg: 32px
  xl: 56px
rounded:
  none: 0
components:
  concept-figure:
    backgroundColor: "{colors.surfaceSoft}"
    textColor: "{colors.primary}"
    rounded: "{rounded.none}"
    padding: "{spacing.lg}"
  diagram-node:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.none}"
    padding: "{spacing.sm}"
  diagram-flow:
    backgroundColor: "{colors.surfaceSoft}"
    textColor: "{colors.primary}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
  diagram-stack:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    rounded: "{rounded.none}"
    padding: "{spacing.md}"
---

## Overview

Quiet Journal is a monochrome personal writing system. The site should feel like a calm index of thoughts, not a product landing page. Typography and spacing carry the experience; decoration should be rare.

Visual explanations inside posts may use diagrams, but they should feel editorial and quiet. Use simple lines, boxes, arrows, labels, and restrained contrast. Diagrams should clarify an idea without becoming the main visual identity of the site.

## Colors

The palette is pure monochrome.

- **Primary:** black for titles, strong labels, and key strokes.
- **Secondary:** dark gray for body-supporting copy.
- **Muted:** mid gray for metadata and captions.
- **Line:** light gray for dividers and low-emphasis structure.
- **Surface:** white page background.
- **Surface Soft:** very light gray for explanation panels.

Do not add accent colors unless the whole site direction changes. Content diagrams should stay black, white, and gray.

## Typography

Use large type sparingly. Korean headings need controlled line breaks and `word-break: keep-all` to avoid awkward syllable-level wrapping. Body text should stay narrow enough for comfortable reading.

Labels are small, uppercase, and quiet. They provide orientation, not decoration.

## Layout

The site uses generous whitespace and a centered content column. Avoid left/right guide rails and dense ornamental grids. Internal pages should feel like clear rooms, while the home page should act as a simple directory.

Article pages use a structured header with metadata separated from the title. Body copy is narrower than the overall page so long Korean paragraphs remain readable.

## Shapes

Diagram shapes should be simple:

- Thin rectangular nodes.
- Thin connecting arrows.
- Circular loops only when the concept is genuinely cyclical.
- Stacked layers for systems or environments.

Avoid rounded cards, gradients, shadows, decorative blobs, and image-like illustrations.

## Components

### Concept Figure

Use for explanatory diagrams inside posts. It should have a light gray surface, a subtle border, a small caption, and enough padding to breathe.

### Diagram Node

Use for labels inside diagrams. Nodes should be rectangular, high-contrast, and legible at mobile widths.

### Diagram Flow

Use for left-to-right conceptual movement, such as "prompt -> agent -> goal" or "chatbot -> dashboard -> operating system." Flow diagrams should use three to five nodes at most. On mobile, stack the nodes vertically and rotate arrows downward.

### Diagram Stack

Use for layered systems, data pipelines, or operating environments. The last layer may be slightly stronger in weight when it represents the resulting judgment or next action.

## Do's and Don'ts

- Do keep diagrams explanatory and sparse.
- Do preserve monochrome color.
- Do give each diagram a caption.
- Do optimize Korean line breaks manually when needed.
- Don't add decorative icons or colorful accents.
- Don't turn article pages into presentation slides.
- Don't let diagrams overpower the writing.
