# Meadowlane Village

A small, endless, procedurally generated English-countryside village you can walk, fly over and map, built with Three.js and Vite. Cottages, farms, a village green with a fountain, lanes, trees, telephone wires, a drifting sky and a few birds, all streamed in around you from a deterministic seed.

## Run

    npm install && npm run dev      # http://localhost:5173
    npm run build                   # static site in dist/
    npm run preview

## Controls

| Input | Action |
|---|---|
| W A S D / arrows | Move |
| Mouse | Look (click "Let's explore" to lock the pointer; drag to look if locked out) |
| Shift | Boost (run) |
| Space | Jump, or fly up |
| Q / Ctrl | Fly down |
| V | Toggle first / third person |
| F | Toggle flight |
| M or Tab | Detailed map: drag to pan, wheel to zoom, click to drop a waypoint |
| P | Settings: walk / fly / boost speeds, camera distance, look sensitivity |
| Mouse wheel, + / - | Change current speed |
| Esc | Pause |

On touch devices a joystick, jump / down / boost buttons and the top toolbar are shown.

## Layout

- `index.html`: markup for the HUD, menus, map and touch controls.
- `src/main.js`: the world (rendering, chunk streaming, collision, character, map, UI).
- `src/style.css`: styles.
- `public/`: static assets.
- `docs/FEATURE_COMPARISON.md`: notes on how this merges the earlier v1 and v2 worlds.
