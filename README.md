# Ardo Defense

**Ardo Defense** is a browser-based tower defense game with an isometric 2.5D playfield. Enemies march from the west side of the map toward the east along a path; you spend **gold** to build and **upgrade** towers on grass tiles so they never reach the end. Each leak costs **lives**—when lives hit zero, the run ends.

Each new run can use a **procedurally generated path** (orthogonal route from left to right) or fall back to a classic layout, so map shape varies between games. Waves get harder over time; **new tower types unlock** as you reach higher waves (from cheap short-range starters to long-range siege, splash, slow fields, armor-piercing shells, anti-air flak, and continuous beam weapons).

**Campaign mode** ends in victory after clearing **wave 18**; you can then **continue in Endless** mode for high scores. **Endless mode** has no win screen—survive as long as you can.

Opponents include fast scouts, armored brutes, **flying** units (countered by AA towers), **regenerating** creeps, and heavy **boss-tier** enemies that cost multiple lives if they escape. Ground-only siege towers cannot hit flyers. Stronger foes drop more gold when killed.

The HUD supports **light/dark themes**, **wave previews** with threat badges, tower **inspect / upgrade / sell**, per-tower **targeting modes**, manual or **auto-advance waves**, **pause**, **1× / 2× / 3× speed**, and procedural **SFX**.

## How to run

No build step is required. Open `index.html` in a modern desktop or mobile browser, or serve the project folder with any static file server (recommended if you hit browser restrictions loading local assets).

Optional **Firebase / Firestore** integration powers the online **leaderboard** (see `firebase-config.js` and `firestore.rules`). If Firebase is not configured, the game still plays locally.

## Controls

- Pick a tower from the shop, click grass to **place**
- Click a built tower to **inspect**, **upgrade** (up to level 3), change **target mode**, or **sell**
- **Right-click** or **CANCEL** clears placement mode
- **Esc** toggles pause
- Touch: tap the canvas to place or select

## Repository layout

| Path | Purpose |
|------|---------|
| `index.html` | Game UI, canvas rendering, and all gameplay logic |
| `assets/towers/`, `assets/enemies/` | Tower and enemy sprites |
| `firebase-config.js` | Web app config for optional cloud leaderboard |
| `tools/` | Helper scripts (e.g. sprite generation) |

## License

Licensed under the Apache License 2.0; see `LICENSE`.
