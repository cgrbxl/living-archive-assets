# TypeCoach asset pack

A Living Archive application identity for learning touch typing through clear instruction, deliberate repetition, and honest feedback. TypeCoach should feel focused and humane: a practice studio, not an arcade.

## Folders

- `branding/`: application mark and horizontal title lock-up.
- `app-icons/`: launcher and iPhone Home Screen icons. Use 180 px for `apple-touch-icon`; 192/512 px for the web manifest.
- `favicons/`: simplified browser-tab mark at 16/32/48/64 px, SVG, ICO, and Safari mask.
- `icons/svg/`: scalable semantic icons with standard and `-reversed` variants.
- `icons/png/`: exact 24/32/64 px exports for fixed-size surfaces.
- `illustrations/`: editable learning graphics and 1200 px PNG exports.
- `motifs/`: quiet keyboard and keystroke structures for headers, dividers, and empty states.
- `tokens/`: CSS and JSON definitions for the application theme.

## Visual semantics

Navy represents the lesson structure, typed record, and stable keyboard geometry. Orange marks the current key, insertion point, or observation under review. Grey represents upcoming, historical, or inactive practice material.

Orange does not mean “wrong.” Accuracy, corrections, and progress need labels, symbols, and accessible text. Never punish errors with alarming animation.

## Learning boundary

Use repetition, pace, and feedback to support skill development. Do not add lives, streak anxiety, trophies, confetti, leaderboards, countdown pressure, or shame-based error states. Speed follows accuracy and comfort; it is not the only objective.

## Icon selection

`keyboard`, `lesson`, `practice`, `drill`, `accuracy`, `speed`, `progress`, `exercise`, `timer`, `text`, `words`, `punctuation`, `numbers`, `hand-position`, `review`, `goal`, `history`, and `results` cover the primary TypeCoach navigation and practice workflow.

## Suggested web setup

```html
<link rel="icon" type="image/svg+xml" href="/assets/apps/typecoach/favicons/typecoach-favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/apps/typecoach/favicons/typecoach-favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apps/typecoach/app-icons/typecoach-app-icon-180.png">
```

Prefer SVG for responsive controls. Keep visible labels for primary navigation and give every semantic icon an accessible name.
