# Diamond

A daily MLB series prediction game. Pick how every active series plays out — game by game — before the first pitch. Come back each day to see your results painted green or red, then lock in your updated read on the remaining games.

Built as part of the Dugout sports intelligence system.

---

## How It Works

Every week MLB teams play 2, 3, or 4-game series. Diamond pulls the live weekly schedule and lets you call each game before it's played.

**Day 1 (series opens)**
All games in the series are available. Pick a winner for each game and lock in your reads before first pitch.

**Each following day**
Yesterday's results are revealed — green if you called it, red if you didn't. The next game opens for a new pick. You can stay with your read or adjust based on what you saw.

**Final day**
All results are in. Your full pick history for the series is graded.

---

## Features

- Live MLB schedule pulled automatically every week
- Team logos, win-loss records, and probable pitchers per game
- Game-by-game pick mechanic with daily reveal
- Green / red result painting on completed games
- Series outcome tracker — sweep, split, or in-progress score
- Weekly accuracy stats with running win rate
- Picks saved locally and persist across sessions
- Auto-refreshes at midnight when results come in
- Works on desktop and mobile

---

## Tech

Single HTML file. No framework, no build step, no dependencies.

Data from the public MLB Stats API (`statsapi.mlb.com`). No API key required.

Picks stored in `localStorage`. Nothing leaves your browser.

---

## Deployment

Hosted on GitHub Pages.

Live at: `https://luffysbigbrother.github.io/diamond`

To run locally, serve the file from any static server — opening it directly as a file will block the MLB API due to CORS.

```bash
# Quick local server (Python)
python3 -m http.server 8000
# Then open http://localhost:8000
```

---

## Part of Dugout

Diamond is one piece of the Dugout sports intelligence system — a personal suite of tools built around how baseball is actually watched, tracked, and argued about.
