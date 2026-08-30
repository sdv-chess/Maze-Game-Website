# Deep Delve 🌀

*A maze you carry with you.*

Deep Delve is a browser-based maze game with no backtracking — you get a limited budget of hints and "unwinds" to escape dead ends, and once you reach the torch, your run is saved to your account for good. Built as a single-page app in vanilla HTML/CSS/JS, with [Supabase](https://supabase.com) handling accounts and progress storage.

**[▶ Play Deep Delve](https://sdv-chess.github.io/Maze-Game-Website/)**

---

## Features

- **Procedurally generated mazes** — a new layout every run, in Small, Medium, or Large presets, or a fully Custom size (5–300 cells per side)
- **No-backtrack gameplay** — walk into a dead end and the run is over, unless you spend one of your limited **Unwinds** (step back one cell) or use a **Peek** (briefly reveals the way forward). Budgets scale with maze size
- **Level Mode** — an endless staircase of mazes that grows wider, taller, and tougher every level, with jump-to-level navigation
- **Sprint & Marathon modes** — an 8×8 maze against a 1-minute clock, or a sprawling 60×60 grind
- **Fog of war** — optional setting that only lights the cave near your character, leaving the rest dark until explored
- **Challenge a friend** — pack your current maze (layout + settings, no progress) into a shareable link; whoever opens it drops straight into the same maze
- **Replay & practice** — step or play back any solved run, then click into the maze to practice from any point, separate from your recorded path
- **Accounts & progress** — sign in to save solve history (grouped by maze category), resume mazes in progress, and sync across devices
- **Achievements** — badges across bronze, silver, gold, platinum, diamond, and mythic ranks, plus unlockable flairs and cosmetic character/theme unlocks
- **Streaks & insights** — daily solve streaks and an insights view summarizing progress across maze types
- **Sound & accessibility touches** — footstep, win, and dead-end sound effects (toggleable), keyboard (WASD/arrows) and swipe controls, and an in-app "How to Play" guide

## Tech stack

- Vanilla HTML, CSS, and JavaScript — no build step, no framework
- HTML5 Canvas for maze rendering and animation
- [Supabase](https://supabase.com) for authentication and storing accounts, solve history, and progress
- Deployed via **GitHub Pages**

## Running locally

Deep Delve is a single static HTML file, so there's nothing to build:

1. Clone the repo:
   ```bash
   git clone https://github.com/sdv-chess/Maze-Game-Website.git
   cd Maze-Game-Website
   ```
2. Open `index.html` directly in a browser, or serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
   then visit `http://localhost:8000`.

Account features (sign-in, saved progress, badges) require a connected Supabase project. Without one, the game still works in guest mode, but progress won't be saved.

## Project structure

```
index.html   # the entire app — markup, styles, and game logic
```

## Feedback

There's a feedback form built into the app (Feedback screen), or you can reach out directly at sairajvernekar@yahoo.com.

## License

No license has been specified yet — all rights reserved by default.
