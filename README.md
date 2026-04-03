# Ardo Defense

**Ardo Defense** is a browser-based tower defense game with an isometric 2.5D playfield. Enemies march from the west side of the map toward the east along a path; you spend **gold** to build and upgrade towers on grass tiles so they never reach the end. Each leak costs **lives**—when lives hit zero, the run ends.

Each new run can use a **procedurally generated path** (orthogonal route from left to right) or fall back to a classic layout, so map shape varies between games. Waves get harder over time; **new tower types unlock** as you reach higher waves (from cheap short-range starters to long-range siege, splash, slow fields, armor-piercing shells, and continuous beam weapons).

Opponents include fast scouts, armored brutes, **flying** units, **regenerating** creeps, and heavy **boss-tier** enemies that cost multiple lives if they escape. Stronger foes drop more gold when killed. The HUD supports **light/dark themes**, manual or **auto-advance waves**, and **game speed** control.

## How to run

No build step is required. Open `index.html` in a modern desktop or mobile browser, or serve the project folder with any static file server (recommended if you hit browser restrictions loading local assets).

Optional **Firebase / Firestore** integration powers the online **leaderboard** (see `firebase-config.js` and `firestore.rules`). If Firebase is not configured, the game still plays locally.

## Repository layout

| Path | Purpose |
|------|---------|
| `index.html` | Game UI, canvas rendering, and all gameplay logic |
| `assets/towers/`, `assets/enemies/` | Tower and enemy sprites |
| `firebase-config.js` | Web app config for optional cloud leaderboard |
| `tools/` | Helper scripts (e.g. sprite generation) |

## License

Licensed under the Apache License 2.0; see `LICENSE`.
