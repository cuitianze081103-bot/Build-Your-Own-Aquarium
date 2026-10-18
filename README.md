# Aquarium Workshop

An English-language interactive aquarium built with HTML, CSS, and Canvas. Shape the sand, plant a garden, fill the tank, choose up to six fish, feed them, and explore.

This repository starts from the original side-view version with the sand tool background removed.

## Run locally

Open `index.html` in a browser. No build or package installation is required.

For an HTTP preview, serve this directory with a static server, for example:

```sh
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Controls

- Hold and move the sand bag over the tank to add depth; use the shovel to shape it.
- Drag a plant into the sand. Drag its top to resize, click to change its color, or drag it to Remove.
- Hold the faucet to fill the tank.
- Choose Fish Type, Color, Size, and Quantity, then select Add Fish.
- Select Feed Fish and click the water. Fish swim toward the food.
- In free play, move slowly to attract fish, click to make ripples, and click a pufferfish to inflate it.
- Edit / Done changes editing modes. Save Aquarium downloads a PNG; Restart begins again.
- With the tank focused, arrow keys move the interaction point and Space uses the current tool.

## Check changes

Node.js 20 or later is recommended. There are no npm dependencies.

```sh
npm run check
npm test
```

The interaction checks cover locked steps, sand, plant placement, water, fish limits, feeding, automatic progression, Edit/Done, and Restart.

## Working with Codex

All Codex changes must be made on a `codex/<task>` branch and proposed through a pull request to `main`. The owner decides when to merge. See [AGENTS.md](AGENTS.md).

The initial project import is on `codex/setup-aquarium`. No automatic deployment or repository visibility changes are configured.

## Files

- `index.html`: page layout and English controls.
- `style.css`: responsive light/dark interface.
- `app.js`: rendering and the six-step interaction flow.
- `tests/aquarium.test.cjs`: dependency-free state/interaction checks.
