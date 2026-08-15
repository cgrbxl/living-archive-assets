# The Living Archive UI Asset Pack

Version 1.2.0. Developer-ready visual assets for Kingdom interfaces. SVG files are the editable source of truth; PNG files are exact-size convenience exports for platforms that cannot consume SVG.

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

## Repository map

| Folder | What it contains | Intended use |
| --- | --- | --- |
| `logos/` | Primary Living Archive mark, reversed mark and horizontal lock-up | Global mastheads, sign-in screens, documentation covers and institutional identity |
| `app-icons/` | General-purpose square launcher icons | App launchers and generic Living Archive shortcuts when no app-specific icon exists |
| `favicons/` | General favicon files, Safari mask and themed favicon families | Browser tabs, bookmarks and browser history; use exact 16/32/48/64 px files when requested |
| `page-role-icons/svg/` | Original scalable page and role icon masters | Responsive navigation, page headers and role cards; prefer SVG in web applications |
| `page-role-icons/png/` | Exact PNG exports of original role icons | Native tools, documents and systems that cannot display SVG |
| `theme-icons/svg/` | Expanded semantic icon vocabulary with standard and `-reversed` variants | Kingdom-wide interfaces requiring archive, governance, financial, knowledge or institutional concepts |
| `theme-icons/png/` | Theme icon exports at 32, 64 and 128 px | Fixed-size navigation, launchers, presentations and documentation |
| `motifs/` | Open arcs, layers, dividers and constellation structures | Quiet structural decoration, empty states and section separators—not primary controls |
| `seals/` | Main institutional seal and themed seal families | Constitutional documents, provenance panels, audit records and formal institutional contexts |
| `tokens/` | Base colors and controlled theme variants in CSS and JSON | Shared design variables; applications should import a coherent theme rather than copying colors manually |
| `apps/` | Complete, application-specific sub-packs | Each app folder contains its own branding, launcher icons, favicons, controls, diagrams, tokens and local README |
| `manifest.json` | Machine-readable list of sizes, themes and application packs | Build tooling, asset browsers, validation and automated discovery |
| `preview-role-icons.png` and `preview-theme-icons.png` | Contact sheets | Human review only; do not use these composite sheets as production UI assets |

## Choosing the correct asset

1. Check `apps/<application-name>/` first. App-specific assets take precedence inside that application.
2. Use `page-role-icons/` for the original canonical roles and pages.
3. Use `theme-icons/` when a broader semantic concept is needed.
4. Use a seal only for formal institutional identity, never as an ordinary button icon.
5. Use motifs only as low-weight structural punctuation.
6. If the required concept does not exist, extend this pack; do not import a visually unrelated icon family.

For web interfaces, reference SVG directly where practical. For native launchers, favicons and iPhone Home Screen icons, use the supplied exact PNG size. Never enlarge a smaller PNG when a larger source or SVG exists.

## Expanded Kingdom theme library (v1.1)

The `theme-icons/` directory adds a broader semantic vocabulary while preserving the same open-arc frame, disciplined line weight, navy structure, and orange insight nodes. File names use lowercase kebab-case English terms. Correct canonical spellings are used: `bureaucracy`, `intelligence`, and `gate`.

Included themes: archive, library, catalogue, council, kingdom, king, minister, court, app, registry, capabilities, agent, officer, intelligence, ai, gate, knowledge, bureaucracy, rules, constitution, law, economy, financial, investor, governance, provenance, memory, evidence, auditor, treasury, observatory, ministry, legislation, sovereignty.

The `favicons/themes/` directory contains intentionally simplified browser-tab variants for twelve major application families. Choose the favicon matching the application's primary institutional identity; do not use a detailed role icon as a 16 px favicon.

The `seals/themes/` directory contains formal and reversed seals for archive, council, kingdom, court, registry, constitution, law, treasury, knowledge, and governance contexts. Seals indicate institutional identity, not automatic approval or legal authority.

The `tokens/themes.css` and `tokens/themes.json` files provide six controlled atmosphere variants. They vary emphasis only within the approved visual language. They are not separate brands and must not be mixed arbitrarily within one application.

## Economic Model Runner application pack (v1.2)

`apps/economic-model-runner/` contains the complete identity and explanatory visual system for the economic model runner and scenario game. Its purpose is to make economic relationships, policy choices, shocks, feedback and uncertainty understandable without turning the product into a trading terminal or arcade game.

The pack includes:

- app branding and horizontal title lock-up;
- launcher icons, including a dedicated 180 px iPhone Home Screen icon;
- browser favicons and Safari mask;
- model controls and economic concepts in SVG plus 24/32/64 px PNGs;
- reusable infographics for circular flow, policy transmission, scenario comparison, sector balances and the scenario-learning loop;
- app-specific CSS and JSON tokens;
- a local README with integration examples and the boundary between useful game mechanics and manipulative gamification.

Within this application, orange indicates the active intervention, scenario, shock or user choice. It does **not** mean that the result is beneficial. Outcomes, assumptions and uncertainty must always be explained with labels and evidence.
