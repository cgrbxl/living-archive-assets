# SaiLearn asset pack

A Living Archive application identity for courses, study sheets, quizzes, and exams. Naval and marine forms provide orientation—charts, routes, sails, compass points, waves, and harbours—while the learning controls remain immediately understandable.

## Folders

- `branding/`: application mark and horizontal title lock-up.
- `app-icons/`: launcher and iPhone Home Screen icons. Use 180 px for `apple-touch-icon`; 192/512 px for the web manifest.
- `favicons/`: simplified browser-tab mark at 16/32/48/64 px, SVG, ICO, and Safari mask.
- `icons/svg/`: scalable semantic icons with standard and `-reversed` variants.
- `icons/png/`: exact 24/32/64 px exports for fixed-size surfaces.
- `illustrations/`: editable learning-voyage graphics and 1200 px PNG exports.
- `motifs/`: chart-grid and wave structures for headers, dividers, and empty states.
- `tokens/`: CSS and JSON definitions for the application theme.

## Visual semantics

Navy represents the charted course: curriculum, assessment structure, and recorded work. Orange marks the current waypoint, question, or item under review. Grey represents completed wakes, reference material, and inactive routes.

Naval language is a metaphor for orientation, not hierarchy or combat. Avoid warships, weapons, military insignia, piracy, rank badges, storms as punishment, or “sink/fail” language.

## Learning boundary

Quizzes and exams should communicate scope, time, completion, and evidence without manufacturing urgency. Do not use lives, streak anxiety, trophies, confetti, countdown pressure, or competitive ranking. A result is a record for review, not a verdict on the learner.

## Icon selection

`dashboard`, `courses`, `lessons`, `study-sheets`, `quiz`, `exam`, `questions`, `answers`, `flashcards`, `notes`, `library`, `progress`, `results`, `review`, `schedule`, `compass`, `chart-course`, `lighthouse`, `anchor`, and `certificate` cover the principal learning and marine-navigation vocabulary.

## Suggested web setup

```html
<link rel="icon" type="image/svg+xml" href="/assets/apps/sailearn/favicons/sailearn-favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/apps/sailearn/favicons/sailearn-favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apps/sailearn/app-icons/sailearn-app-icon-180.png">
```

Use marine motifs as low-weight structure and keep quiz, exam, notes, and sheet icons literal enough to scan quickly.
