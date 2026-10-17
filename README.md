# Goblin Hoard 👺🪙

A tiny idle clicker game: poke a goblin, steal gold, and fund goblin schemes
that loot for you while you're not looking.

Built as a single self-contained `index.html` — no build step, no dependencies.

## How to play

- **Poke the goblin** (click / tap / Enter / Space) to steal gold.
- Spend gold in the **Shenanigans** shop:
  - Click upgrades raise gold per poke.
  - Passive upgrades earn gold every second on their own.
- Every purchase makes that upgrade 15% more expensive.
- Progress **auto-saves** in your browser (localStorage) every few seconds
  and when you close the tab.
- While you're away, your crew keeps looting — up to **8 hours** of offline
  earnings, paid out the next time you open the game.
- **Reset hoard** (footer) wipes your progress and starts over.

## Run locally

Open `index.html` in any modern browser. That's it.

## Deployment

Every push to `main` auto-deploys to GitHub Pages via
`.github/workflows/deploy-pages.yml`.

## Tech notes

- One HTML file: inline CSS + vanilla JS, inline SVG goblin.
- Coin sound is synthesized with the WebAudio API (no audio assets);
  the mute preference is persisted.
- Saves live in `localStorage` under `goblin-hoard-save-v1`.