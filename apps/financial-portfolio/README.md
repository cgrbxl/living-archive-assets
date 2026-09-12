# Financial Portfolio asset pack

A Living Archive application identity for understanding holdings, allocation, performance, income, risk, and portfolio decisions. It should feel like a calm archival instrument: evidence-led, legible, and deliberate—not a brokerage terminal or a game.

## Folders

- `branding/`: application mark and horizontal title lock-up.
- `app-icons/`: launcher and iPhone Home Screen icons. Use 180 px for `apple-touch-icon`; 192/512 px for the web manifest.
- `favicons/`: simplified browser-tab mark at 16/32/48/64 px, SVG, ICO, and Safari mask.
- `icons/svg/`: scalable semantic icons with standard and `-reversed` variants.
- `icons/png/`: exact 24/32/64 px exports for fixed-size surfaces.
- `illustrations/`: editable explanatory graphics and 1200 px PNG exports.
- `motifs/`: quiet structural graphics for empty states, dividers, and portfolio headers.
- `tokens/`: CSS and JSON definitions for the application theme.

## Visual semantics

Navy represents recorded structure: accounts, holdings, baselines, and evidence. Orange identifies the point currently being examined or changed. Grey represents historical periods, comparison series, and inactive allocations.

Orange is not a gain signal. Do not imply profit/loss, safety/risk, or buy/sell with colour alone. Pair outcomes with plain labels, signed numbers, arrows, and accessible descriptions. This pack intentionally avoids red/green market-terminal conventions.

## Product boundary

Use the assets to help people understand what they own, why it changed, and how uncertainty is distributed. Do not add candlestick wallpaper, rockets, trophies, coins, flashing tickers, countdowns, confetti, or urgency cues. Portfolio decisions should remain reviewable and reversible.

## Icon selection

| Icon | Intended meaning |
| --- | --- |
| `portfolio` | application home or portfolio container |
| `overview` | summary dashboard |
| `accounts` | custody, wrappers, or connected accounts |
| `holdings` | owned positions |
| `allocation` | distribution by asset class or category |
| `performance` | change over time |
| `benchmark` | comparison against a reference |
| `transactions` | purchases, sales, transfers, and ledger activity |
| `dividends` | distributions received from holdings |
| `income` | portfolio cash income |
| `cash` | cash balance or reserve |
| `risk` | uncertainty, exposure, or risk review |
| `rebalance` | target-allocation adjustment |
| `watchlist` | monitored assets not necessarily held |
| `markets` | market context, never a live-trading call to action |
| `goals` | portfolio objective or target |
| `reports` | statements, evidence, and exports |
| `tax-lots` | acquisition lots and tax records |

## Suggested web setup

```html
<link rel="icon" type="image/svg+xml" href="/assets/apps/financial-portfolio/favicons/financial-portfolio-favicon.svg">
<link rel="icon" type="image/png" sizes="32x32" href="/assets/apps/financial-portfolio/favicons/financial-portfolio-favicon-32.png">
<link rel="apple-touch-icon" sizes="180x180" href="/assets/apps/financial-portfolio/app-icons/financial-portfolio-app-icon-180.png">
```

Prefer SVG for responsive interface icons. Keep visible navigation labels and give semantic icons an accessible name. Decorative motifs use empty alternative text.
