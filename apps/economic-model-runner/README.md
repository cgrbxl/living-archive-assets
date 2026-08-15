# Economic Model Runner asset pack

A Living Archive application identity for running economic models, comparing scenarios and exploring policy trade-offs. The interface may use game mechanics, but must feel like a serious scenario laboratory—not a casino, trading terminal or strategy game.

## Folders

- `branding/`: app mark and horizontal title lock-up. Use the SVG masters wherever possible.
- `app-icons/`: launcher and iPhone Home Screen icons. Use the 180 px file for `apple-touch-icon`; 192/512 for the web manifest.
- `favicons/`: simplified browser-tab icons at 16/32/48/64 px, SVG and Safari mask.
- `icons/svg/`: scalable semantic controls and model concepts, including reversed navy-tile variants.
- `icons/png/`: exact exports for 24, 32 and 64 px contexts.
- `infographics/svg/`: editable source diagrams for model explanations and empty states.
- `infographics/png/`: 1200 px reference exports for documents and fixed-image surfaces.
- `tokens/`: CSS and JSON definitions for the app's controlled visual theme.

## Visual semantics

Navy represents model structure, accounting identities and baselines. Orange represents an active scenario, intervention, shock or human choice. Grey represents history, comparison or inactive structure. Orange must not imply that an outcome is good; results need explicit labels and evidence.

## Game-design boundary

Use turns, scenarios, constraints and feedback to aid learning. Do not add coins, trophies, loot, gambling motifs, confetti, urgent countdowns or false certainty. The objective is understanding trade-offs, not maximising a fictional score. Keep assumptions, model limitations and uncertainty visible.

## Suggested web setup

```html
<link rel="icon" type="image/svg+xml" href="/assets/apps/economic-model-runner/favicons/economic-model-runner-favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/apps/economic-model-runner/favicons/economic-model-runner-favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apps/economic-model-runner/app-icons/economic-model-runner-app-icon-180.png">
```

Manifest icon entries should reference the 192 and 512 px PNG files and use `display: standalone`. Delete and recreate an existing iPhone Home Screen shortcut after changing its icon because iOS may retain the older image.
