# Wargame asset pack

A Living Archive application identity for the configurable, hex-based WWII wargame. The game is about operational command: issuing orders, maintaining command and supply, reading terrain, and reviewing deterministic outcomes. The visual system should feel like a clear staff map—not propaganda, militaria, or an arcade shooter.

The application mark preserves the existing two-symbol identity: an Archive Orange flat-top hexagon for the map grid, with an Archive Navy advance arrow knocked out for orders-driven movement.

## Folders

- `branding/`: application mark and horizontal title lock-up.
- `app-icons/`: launcher, iPhone Home Screen, and PWA maskable icons.
- `favicons/`: browser-tab mark at 16/32/48/64 px, SVG, ICO, Safari mask, and web manifest.
- `icons/svg/`: semantic controls and game concepts with standard and `-reversed` variants.
- `icons/png/`: exact 24/32/64 px exports for fixed-size UI surfaces.
- `illustrations/`: editable explanatory diagrams and 1200 px PNG exports.
- `motifs/`: quiet hex-grid, counter, and operational-route structures.
- `social/`: 1200×630 link-preview artwork in SVG and PNG.
- `tokens/`: Living Archive brand tokens plus the game’s existing side and terrain semantics.

## Visual semantics

Archive Navy provides application structure. Archive Orange identifies the active order, selected route, or decision under review. Warm white and grey carry historical and inactive structure.

Blue and red are game-side identifiers only. They do not encode moral alignment or historical nationality. Terrain colours describe the board and must not be repurposed for status. Never communicate command, supply, morale, or readiness through colour alone; retain the game’s symbols, labels, pips, and patterns.

## Historical and sensitivity boundary

Use abstract operational cartography, generic counters, routes, terrain, and command relationships. Do not introduce national flags, political symbols, unit insignia, medals, uniforms, portraits, weapons-as-branding, propaganda typography, or celebratory destruction. The app mark must remain faction-neutral.

## Icon vocabulary

`battle-map`, `scenario`, `orders`, `command-net`, `units`, `group`, `objective`, `movement`, `attack`, `air-support`, `reinforcements`, `airborne`, `supply`, `depot`, `transport`, `entrench`, `refit`, `morale`, `terrain`, `road`, `undo`, `save-game`, `replay`, `execute-orders`, `take-control`, and `next-unit` cover the current prototype’s primary controls and rule concepts.

## Suggested web setup

```html
<link rel="icon" type="image/svg+xml" href="/assets/apps/wwiigame/favicons/wwiigame-favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/apps/wwiigame/favicons/wwiigame-favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apps/wwiigame/app-icons/wwiigame-app-icon-180.png">
<link rel="manifest" href="/assets/apps/wwiigame/favicons/site.webmanifest">
```

Use SVG for responsive navigation and panels. Keep visible labels on the dense command interface and treat motifs as low-weight structure rather than controls.
