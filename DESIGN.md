---
name: Dra. Yeda Karolinne
description: Otomodelação link page where the client's palette drifts slowly behind an arched mirror that holds the real clinic video.
colors:
  slate: "#6A6866"
  slate-press: "#5D5B59"
  taupe: "#A18A78"
  sand: "#CFC3B3"
  mist: "#ECE5DB"
  on-slate: "#F7F3EE"
  ink: "#2B2725"
  ink-soft: "#3D3835"
  glass: "rgba(250,247,242,.66)"
  glass-hover: "rgba(250,247,242,.84)"
  line: "rgba(255,255,255,.65)"
typography:
  display:
    fontFamily: "Italiana, serif"
    fontSize: "clamp(2.3rem, 6.4vw, 5.4rem)"
    fontWeight: 400
    lineHeight: 0.98
    letterSpacing: "0.005em"
  body:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "clamp(.98rem, 1.3vw, 1.12rem)"
    fontWeight: 400
    lineHeight: 1.45
  title:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "1.02rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.01em"
  title-action:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "1.1rem"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.01em"
  label:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "0.84rem"
    fontWeight: 400
    lineHeight: 1.3
  small:
    fontFamily: "Jost, system-ui, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 400
    lineHeight: 1.6
rounded:
  icon: "14px"
  row: "20px"
  mirror-foot: "30px"
  pill: "999px"
spacing:
  row-gap: "10px"
  stack-gap: "22px"
  stack-gap-wide: "28px"
  row-inset: "10px 18px 10px 10px"
components:
  link-row:
    backgroundColor: "{colors.glass}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "{spacing.row-inset}"
    height: "64px"
  link-row-hover:
    backgroundColor: "{colors.glass-hover}"
  link-row-primary:
    backgroundColor: "{colors.slate}"
    textColor: "{colors.on-slate}"
    typography: "{typography.title-action}"
    rounded: "{rounded.row}"
    padding: "{spacing.row-inset}"
    height: "72px"
  link-row-primary-hover:
    backgroundColor: "{colors.slate-press}"
  icon-tile:
    backgroundColor: "rgba(207,195,179,.55)"
    textColor: "{colors.slate}"
    rounded: "{rounded.icon}"
    size: "44px"
  sound-control:
    backgroundColor: "rgba(43,39,37,.38)"
    textColor: "#FFFFFF"
    rounded: "{rounded.pill}"
    size: "44px"
  footer-pill:
    backgroundColor: "rgba(250,247,242,.55)"
    textColor: "{colors.ink}"
    typography: "{typography.small}"
    rounded: "{rounded.pill}"
    padding: "4px 12px"
---

# Design System: Dra. Yeda Karolinne

## Overview

**Creative North Star: "The Mirror in Moving Light"**

A calm, fluid surface. The client's four tones (mist, sand, taupe, slate) never sit still as a flat fill: they drift as large soft blobs under a fine grain, slowly enough to read as light shifting in a room rather than as animation. Against that moving ground one object holds still and carries all the proof: an arched mirror, framed in a translucent bezel, playing the real clinic clip in which the patient sees herself in a mirror.

Everything else is quiet and light. The name is set large in a high-contrast hairline serif; every other word is a clean geometric sans. Link rows are pale translucent panes with a white hairline edge, and only the WhatsApp row is solid. Density is low, one column on phones, two on desktop (words left, mirror right).

**Key Characteristics:**
- Fixed, slowly drifting mesh gradient of the client palette with grain; never a solid background.
- One arched mirror holding the real video; the only framed object on the page.
- Translucent pale link rows with hairline white borders and soft-square icon tiles.
- A single solid slate row for the one action (WhatsApp).
- Italiana for the name only; Jost for everything else.

## Colors

A warm, desaturated stone palette taken directly from the client's brand colours, with one deeper ink for text.

### Primary
- **Mirror Slate** (#6A6866): the solid fill of the one action row (WhatsApp), the mirror's backing before the video paints, icon strokes on pale rows, the selection highlight. Pressed/hover deepens to **Slate Press** (#5D5B59).

### Secondary
- **Warm Taupe** (#A18A78): lives only in the drifting ground (two of the four blobs) and the scrollbar thumb. It is the darkest position the ground's text must survive.

### Neutral
- **Sand** (#CFC3B3): the ground's mid tone, the page's base fill and theme colour, and the tint of icon tiles at 55% opacity.
- **Mist** (#ECE5DB): the ground's lightest blob and the top of the base gradient; selection text.
- **Ink** (#2B2725): all text on the ground and on pale rows: name, line, row labels, footer. Chosen because it holds legible contrast against pure taupe, the ground's darkest drift.
- **Ink Soft** (#3D3835): row sub-lines.
- **On-Slate** (#F7F3EE): text, icons and chevrons on the solid slate row; focus ring colour over the video.
- **Glass** (rgba(250,247,242,.66), hover .84): the translucent fill of link rows.
- **Hairline** (rgba(255,255,255,.65)): the 1px edge on rows and the mirror bezel.

### Named Rules
**The Moving Ground Rule.** The page ground is the drifting four-blob gradient with grain, fixed behind content. Never replace it with a solid colour or a static image.

**The One Solid Rule.** Exactly one surface is solid slate: the primary action. Every other row is translucent glass.

**The Darkest Drift Rule.** Any text that sits directly on the ground uses Ink (#2B2725) and must pass contrast against pure taupe (#A18A78). Small text that can drift over the slate blob gets a pale pill behind it (as the footer does).

## Typography

**Display Font:** Italiana (with serif fallback), self-hosted woff2
**Body Font:** Jost (with system-ui, sans-serif fallback), self-hosted variable woff2, weights 300 to 600

**Character:** A tall, hairline display serif with the poise of an engraved mirror frame, against a calm geometric sans that keeps every action plain and readable.

### Hierarchy
- **Display** (400, clamp(2.3rem, 6.4vw, 5.4rem), 0.98): the doctor's name only, balanced wrap.
- **Body** (400, clamp(.98rem, 1.3vw, 1.12rem), 1.45, max 30ch): the one-line specialty under the name; the specialty word itself takes weight 500.
- **Title** (500, 1.02rem, 1.2, +0.01em): link row labels. The action row steps up to 1.1rem.
- **Label** (400, .84rem, 1.3): row sub-lines, single line with ellipsis.
- **Small** (400, .8rem, 1.6): footer.

### Named Rules
**The One Name Rule.** Italiana sets the name and nothing else. Labels, lines, controls and footers are Jost.

**The Sentence Case Rule.** No uppercase tracking labels; every string is sentence case at its natural size.

## Layout

Single centred column on phones: name and line, then the mirror (width min(66vw, 46svh × 9/16 + 20px, 360px)), then the link list (max 460px), then the footer, stacked with a 22px gap. Page padding is clamp(16px, 5vw, 56px) horizontally and respects safe-area insets; content width caps at 1120px.

From 900px: a two-column grid. The left column holds name, line, links (max 440px) and footer, left-aligned; the mirror spans all rows on the right at about 80svh tall (capped at 820px), vertically centred. Column gap clamp(56px, 8vw, 128px), row gap 28px.

Rows are spaced 10px apart. The first viewport on a phone must show the name, the line, the mirror and the WhatsApp row.

## Elevation & Depth

A light, layered hybrid. Depth comes first from translucency over the moving ground, second from soft, low-contrast, negatively spread shadows tinted with Ink. There are no hard edges or offset shadows.

### Shadow Vocabulary
- **Mirror lift** (`box-shadow: 0 30px 60px -30px rgba(43,39,37,.45), 0 10px 22px -14px rgba(43,39,37,.3)`): the mirror only; it is the one object that stands off the ground.
- **Row rest** (`box-shadow: 0 1px 0 rgba(255,255,255,.5) inset, 0 8px 20px -14px rgba(43,39,37,.35)`): link rows; the inset top line reads as a glass edge catching light.
- **Row hover** (`box-shadow: 0 1px 0 rgba(255,255,255,.6) inset, 0 14px 26px -14px rgba(43,39,37,.4)`): paired with a 2px lift.

### Named Rules
**The Blur Over Film Rule.** backdrop-filter (blur 8px) is used only for controls that sit over the video. Link rows get their glass look from a translucent fill, not blur.

## Shapes

Soft and rounded, with one signature silhouette. The mirror is an arch: a fully rounded top (999px) over gently rounded feet (30px outer, 22px on the inner glass), set inside a 9px (11px desktop) translucent bezel with a hairline white edge. Link rows use 20px corners; icon tiles inside them use 14px soft squares. Controls and the footer are full pills or circles (999px / 50%). Borders are always 1px white hairlines.

## Components

### Link Rows
Calm, pale and touchable.
- **Shape:** 20px corners, 1px hairline white border, min-height 64px.
- **Default:** Glass fill, Ink label, Ink Soft sub-line, slate soft-square icon tile on the left (44px, 14px radius, sand at 55%), slate chevron on the right at 70% opacity.
- **Hover / Active:** fill goes to Glass hover, the row lifts 2px with a deeper shadow, the chevron slides 3px right and becomes fully opaque; active presses back to 0 with scale .99. Transitions .35s on the expo-out curve.
- **Primary (WhatsApp):** solid Mirror Slate, min-height 72px, On-Slate text and icon, icon tile at 14% white, border at 25% white; hover deepens to Slate Press.
- **Icons:** 22px stroked SVG line icons at 1.5 stroke, round caps and joins.

### The Arched Mirror (signature)
The video frame. Arch silhouette with a translucent bezel (rgba(250,247,242,.22)), slate backing, a faint diagonal sheen over the glass, and the Mirror lift shadow. It is the only element with an entrance: it rises 16px and scales from .97 over about 1.3s once the page is ready. Inside it sit two controls:
- **Progress hairline:** 2px white line (30% track, 90% fill) across the foot of the video, scaling with playback.
- **Sound control:** 44px circle, Ink at 38% with an 8px backdrop blur, white hairline, white 20px muted/unmuted line icon; hover darkens to 60%, press scales to .94; focus ring On-Slate.

### Footer Pill
Small Jost text in Ink on a pale pill (rgba(250,247,242,.55), 4px 12px), so it stays legible wherever the ground drifts.

## Do's and Don'ts

### Do:
- **Do** keep the ground as the fixed, slowly drifting four-blob gradient (26s to 38s per blob, alternate, ease-in-out) with grain at 40%, and stop the drift under prefers-reduced-motion.
- **Do** keep exactly one solid slate row, for the primary action.
- **Do** set text on the ground in Ink (#2B2725) and test it against pure taupe; back small text with a pale pill when it can cross the slate blob.
- **Do** use the expo-out curve (cubic-bezier(.16,1,.3,1)) for state transitions and the mirror's entrance.
- **Do** frame the real video in the arched mirror; it is the page's proof.

### Don't:
- **Don't** put the page on a solid background colour.
- **Don't** make link rows heavy or decorative: no solid fills beyond the primary, no thick borders, no hard or offset shadows.
- **Don't** apply backdrop-filter blur outside controls that sit over the video.
- **Don't** use Italiana for anything but the name.
