---
version: alpha
name: goofee-9p — Contents
description: A personal writing & portfolio space. Editorial, serif, generous whitespace, warm monochrome with a single restrained terracotta accent. Plain and understated, never sentimental.
colors:
  paper: "#FBFAF8"
  paper-raised: "#F4F1EA"
  ink: "#1A1714"
  ink-soft: "#57534C"
  ink-quiet: "#8E897F"
  line: "#E5E0D6"
  line-strong: "#CFC9BC"
  accent: "#B5512E"
  accent-deep: "#8F3F22"
  accent-wash: "#F4E8E1"
typography:
  display:
    fontFamily: Newsreader, "Noto Serif KR", serif
    fontSize: 72px
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: -0.021em
  title:
    fontFamily: Newsreader, "Noto Serif KR", serif
    fontSize: 44px
    fontWeight: 500
    lineHeight: 1.12
    letterSpacing: -0.014em
  headline:
    fontFamily: Newsreader, "Noto Serif KR", serif
    fontSize: 28px
    fontWeight: 500
    lineHeight: 1.22
  dek:
    fontFamily: Newsreader, "Noto Serif KR", serif
    fontSize: 21px
    fontWeight: 400
    lineHeight: 1.55
    fontFeature: "'ital' 1"
  body:
    fontFamily: "Noto Serif KR", Newsreader, serif
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.85
  body-sm:
    fontFamily: "Noto Serif KR", Newsreader, serif
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: Inter, sans-serif
    fontSize: 12px
    fontWeight: 600
    lineHeight: 1
    letterSpacing: 0.14em
  meta:
    fontFamily: Inter, sans-serif
    fontSize: 13px
    fontWeight: 500
    letterSpacing: 0.01em
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  xxl: 112px
  measure: 680px
  shell: 1120px
rounded:
  none: 0px
  sm: 3px
  full: 9999px
components:
  link:
    textColor: "{colors.accent}"
  link-hover:
    textColor: "{colors.accent-deep}"
  entry-number:
    textColor: "{colors.accent}"
    typography: "{typography.label}"
  rule-accent:
    backgroundColor: "{colors.accent}"
  row:
    backgroundColor: "{colors.paper}"
  row-hover:
    backgroundColor: "{colors.paper-raised}"
---

# goofee-9p — Contents

A personal space that is one part **writing** (Contents) and one part **portfolio**
(Work). The design exists to make long-form Korean writing feel considered, and to let
selected work stand without noise.

## Overview

Also known as Brand & Style.

The voice is **plain, understated, and confident — never sentimental.** Copy stays factual
and dry; the warmth comes from the typography and paper, not from flowery wording. Pages
should feel like good paper — calm and confident with empty space. Nothing shouts. The
visual identity is **warm monochrome**: a near-white warm paper and a warm near-black ink,
carried almost entirely by typography and hairlines. A single **restrained terracotta
accent** appears rarely — on an entry's number, a link, a short rule — to add a trace of
human warmth, never decoration. If a rule isn't defined, choose the quieter, more
spacious option.

## Colors

Warm neutrals do the work; the accent is a guest, not a host.

- **Paper (#FBFAF8):** A warm off-white that is softer and more human than pure white.
  The foundation of every page.
- **Paper Raised (#F4F1EA):** A slightly deeper warm wash for hover states and quiet
  containment. Used sparingly.
- **Ink (#1A1714):** A warm near-black for headlines and body — permanent, readable, calm.
- **Ink Soft (#57534C):** Secondary prose, deks, and descriptions.
- **Ink Quiet (#8E897F):** Labels, metadata, timestamps.
- **Line (#E5E0D6):** The default warm hairline that structures the page.
- **Accent — Terracotta (#B5512E):** The single accent. A refined, muted clay used only
  for entry numbers, links, and short marker rules. **Restraint is the rule:** at most a
  few accent marks per screen.
- **Accent Deep (#8F3F22):** Hover/active state of the accent.

## Typography

The system pairs a literary serif for everything readable with a quiet grotesque sans for
small labels — the classic editorial contrast.

- **Serif — Newsreader + Noto Serif KR:** Display, titles, headlines, deks, and body. The
  serif carries the writing's voice. Deks (summaries) are set in *italic* serif.
- **Sans — Inter:** Eyebrows, navigation, entry numbers, and metadata only. Always
  UPPERCASE with generous letter-spacing, small and quiet.
- Body runs at a comfortable 18px with 1.85 line-height and a ~680px measure for long
  Korean reading. Display and title sizes are fluid (`clamp`) and the px values above are
  the desktop maxima.
- `word-break: keep-all` is used throughout to keep Korean line-breaks natural.

## Layout

A single, calm reading column.

- **Shell (max 1120px):** Masthead, footer, and wide index lists.
- **Measure (max 680px):** All long-form reading and prose.
- A strict **8px spacing scale** sets the rhythm; sections breathe with `xl`–`xxl`
  vertical space. The home is **content-first**: the latest entry is the largest object on
  the page, the archive follows, and About / Work sit quietly beneath.

## Elevation & Depth

Flat by intent. Hierarchy comes from **type scale, whitespace, and hairlines** — not
shadows. Containment, when needed, is a `paper-raised` wash or a single hairline, never a
box with a drop shadow.

## Shapes

Essentially square. Corners are sharp (`rounded.none`) to read as print; an optional 3px
softening (`rounded.sm`) may be used on interactive controls. The recurring identity motif
is a **short 2px terracotta rule** (~32px wide) used to open a section.

## Components

- **Links:** Inline serif links carry a 1px underline; color shifts to terracotta on
  hover. Standalone "read" links use a trailing arrow (→).
- **Entry number:** A small uppercase sans label (`No. 003`) in terracotta, paired with a
  serif title. (Do not label entries "letters"; use plain numbers / "Contents".)
- **Index row (archive):** A hairline-separated row — number, serif title, date, one-line
  summary. Hover lifts the title to ink and warms the background to `paper-raised`.
- **Eyebrow + accent rule:** Section openers use an uppercase sans eyebrow above a short
  terracotta rule.
- **Pull emphasis:** Key sentences in an entry sit behind a 2px terracotta left border.

## Do's and Don'ts

- Do let whitespace carry the page; when unsure, add space, not lines.
- Do keep the accent rare — an entry number, a link, one rule per section is plenty.
- Don't introduce a second accent color or any shadow.
- Don't set Korean body in sans; the serif is the voice of the writing.
- Don't write sentimental or flowery copy; keep wording plain, factual, and dry.
- Do maintain WCAG AA contrast (terracotta on paper passes for text; pair it with ink for
  anything small).
- Don't mix sharp and rounded corners in the same view.
