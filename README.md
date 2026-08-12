# The Living Archive UI Asset Pack

Version 1.0.0. Developer-ready assets for Kingdom interfaces. The SVG files are the source of truth; PNGs are convenience exports.

## Non-negotiable identity rule

Use **only the icons, marks, seals, and motifs provided in this pack** for Kingdom-branded navigation and identity. Do not generate replacements, redraw them, mix them with third-party icon families, or introduce external heraldic, cyberpunk, fantasy, robot, brain, crown, gavel, or shield imagery. If a required semantic icon is missing, request an addition to this pack using the same construction system.

## Palette

- Archive Navy `#163B66`: structure, navigation, boundaries.
- Archive Orange `#E67E22`: insight, active cognition, human judgement; never a danger color by default.
- Warm White `#F8FAFC`: principal illuminated background.
- Light Archive Grey `#E5E7EB`: layered surfaces and quiet separation.
- Soft Slate `#D9E1EA`: historical context, inactive structure.

Recommended overall balance: 45% warm-white/grey spectrum, 25% navy, 25% orange, 5% neutral accents. This is an atmosphere target, not a per-component quota.

## Logo usage

- `logos/living-archive-mark.svg`: primary transparent mark for light surfaces. Minimum display: 32 px.
- `logos/living-archive-mark-reversed.svg`: contained mark for dark or unpredictable surfaces.
- `logos/living-archive-horizontal.svg`: masthead and sign-in pages. Allow clear space equal to one orange-node diameter. Do not use below 220 px wide.

Do not rotate, skew, add shadows/glows, recolor, close the open circle, remove the central axis, or alter node positions.

## App icons and favicons

Use the exact-size file matching the platform request. App icons have intentionally generous mass for launcher visibility. Browser tabs use the simplified seal in `favicons/`. Include PNG 16/32/48/64 and use `safari-pinned-tab.svg` only as a monochrome pinned-tab mask.

Suggested HTML:

```html
<link rel="icon" type="image/png" sizes="32x32" href="/assets/favicons/favicon-32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/assets/favicons/favicon-16.png">
<link rel="apple-touch-icon" sizes="128x128" href="/assets/app-icons/app-icon-128.png">
<link rel="mask-icon" href="/assets/favicons/safari-pinned-tab.svg" color="#163B66">
```

## Page and role icons

Available: Catalogue, Console, Council, Capabilities, Chart, Kingdom Court, Intelligence Officer, Investment Officer, Janitor, Librarian, Auditor, and Kingdom Gates.

- 24 px: compact navigation and tables.
- 32 px: standard sidebars and controls.
- 64 px: page headers and empty states.
- 128 px: role cards, launchers, and profile panels.
- SVG: preferred for responsive interfaces.
- `-reversed.svg`: navy tile for dark or mixed backgrounds.

Use icons with their supplied open-arc frame. Do not detach the central glyph or combine it with another family. Labels remain visible in primary navigation; icons are not a substitute for clear language.

## Motifs

- `archive-divider.svg`: section breaks, report covers, and modal headings.
- `open-arc-corner.svg`: one corner only per composition; use at low visual weight.
- `constellation-field.svg`: empty states, knowledge-map backgrounds; keep opacity between 8% and 18%.
- `archive-layers.svg`: archive/category headers; never repeat as a dense pattern.

Motifs are structural punctuation, not decoration. Avoid simultaneous use of more than two motifs in one viewport.

## Seals

The institutional seal is for formal records, approvals, audit summaries, constitutional material, and provenance panels. It must not imply legal certification or approval that did not occur. Use the standard seal on light surfaces and the reversed seal on navy. Minimum: 64 px digital, 18 mm print.

## Accessibility and implementation

Decorative marks should use empty alt text. Semantic role icons need a visible text label or accessible name. Do not communicate status through orange alone. Preserve at least 3:1 contrast for large graphical objects and test actual foreground/background pairings. Prefer gentle fades; do not spin, pulse, bounce, or glow these assets.

## File structure

- `logos/`: master marks and masthead.
- `app-icons/`: launcher PNGs.
- `favicons/`: browser-tab assets.
- `page-role-icons/svg/`: scalable light and reversed masters.
- `page-role-icons/png/`: exact-size transparent PNG exports.
- `motifs/`: decorative structural SVGs.
- `seals/`: formal seal SVGs and PNGs.
- `tokens/colors.css`: approved color variables.
- `manifest.json`: machine-readable inventory and rules.
+