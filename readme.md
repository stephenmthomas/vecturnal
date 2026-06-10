# Vecturnal

A browser-based SVG pattern generator. Inspired by an over zealous Figma plugin that had the audacity to charge for basic functionality. Though admittedly, not as refined... but hey - we have LIVE VIEW!

No dependencies, no build step — a single HTML file you can open locally or deploy to GitHub Pages.

https://stephenmthomas.github.io/vecturnal/

## Features

- **Grid system** — generate patterns from 1×1 up to 40×40 clones with configurable X/Y spacing
- **8 base shapes** — circle, rect, triangle, diamond, cross, star, ring, hexagon
- **Custom path** — paste any SVG `d=` path string directly into the shape panel
- **Modifiers** — rotation, opacity, scale, position jitter, and stroke, each with random / noise / proximity modes
- **Color palettes** — coral, teal, purple, amber, blue, mono — with random, sequence, and noise distribution
- **Liveview** — auto-regenerates on any input change when enabled
- **Reseed** — randomize output without changing any settings
- **Export** — downloads the current canvas as a clean `.svg` file
- **Dark / light mode** — toggle in the toolbar, defaults to dark

## Usage

```
git clone https://github.com/stephenmthomas/vecturnal
open index.html
```

Or just download `index.html` and open it in any browser. No server required.

## GitHub Pages

CHECK OUT THE LIVE PAGE HERE:

```
https://stephenmthomas.github.io/vecturnal/
```

## Modifier Modes

| Mode | Behavior |
|------|----------|
| random | Each clone gets an independent random value |
| noise | Smooth organic variation — nearby clones get similar values |
| sequence | Cycles through a defined list in order |
| proximity | Value is determined by distance from a UV focal point |

## Custom Path

Select the **path** shape option and paste any SVG path data into the `d=` field. The path is expected to be centered around the origin (`0,0`) — a path drawn in a 100×100 box should be offset by `-50,-50`. Scale is relative to the grid size setting.

Example — a simple diagonal line centered at origin:
```
M-10,-10 L10,10
```

## License

MIT