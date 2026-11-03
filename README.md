# Word Scramble

A free single-file HTML5 word puzzle: unscramble jumbled letter tiles into
hidden English words.

**Play:** https://shuangyueliao.github.io/word-scramble/

## Features

- 1,117 common 5–7 letter English words across 19 categories (animals, food,
  fantasy, actions…). The bank is anagram-deduplicated — no two words share
  the same set of letters, so a scramble never has two valid answers.
- Two modes: **Blitz** (60 seconds, chain answers for combo bonuses) and
  **Zen** (5 words, no timer).
- Scoring: +100 per word + time bonus + combo bonus; Hint −20 (max 2 per
  word), Skip −30.
- Tap tiles to spell, or just type on a keyboard. Backspace undoes,
  Space reshuffles.
- Wood and Neon themes, synthesized WebAudio sound with a mute toggle.
- Best scores and longest streak saved in localStorage.
- Zero external assets: one `index.html`, no CDN, no images, no fonts,
  no tracking, no external links.

## Run locally

Open `index.html` directly in a browser, or serve it:

    python3 -m http.server 8080

then visit http://localhost:8080/.

## Platform portals

The CrazyGames / GameDistribution SDK loaders activate only on their own
domains (`gameplayStart` / `gameplayStop` are wired for CrazyGames); on any
other host the game runs standalone with no network calls.

## Deploy

GitHub Pages serves the `main` branch root (`.nojekyll` included).
