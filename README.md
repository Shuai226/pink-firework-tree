# Pink Firework Christmas Tree · Zhang Aoyun

A single-file interactive pink firework Christmas tree webpage, cloned from the reference video: pink particle light spots and firework/tree trails, while the original multicolor bauble accents are kept unchanged.

## Features

- Pink cone-shaped tree built from spiral light strands and ~900 glowing pink particles
- Periodic pink fireworks rise and burst in the background; click anywhere to launch one
- Multicolor baubles on branches keep the original palette: green / red / blue / amber
- Radiant top star with rotating light rays
- Left panel shows the source code with lightweight syntax highlighting; right stage runs the animation
- Bottom dedication: script font **Merry Christmas** above **Zhang Aoyun**

## Run

No build step, no dependencies, no CDN. Open `firework-christmas-tree.html` directly in a browser, or serve locally:

```bash
npx serve .
```

## Customize

| What | Where |
| --- | --- |
| Dedication name | `.caption .name` in the HTML |
| Pink palette | `PINK` array in the script |
| Bauble accent colors | `BAUBLE_COLORS` array (kept from the original video) |
| Particle count | `for (let i = 0; i < 900; ...)` in `buildTree()` |
| Spiral strands / turns | `STRANDS`, `TURNS` in `drawHelices()` |
| Auto firework interval | `2.4` seconds in the main loop |

## Tech

- Vanilla HTML / CSS / JavaScript, one self-contained file
- Canvas 2D animation with additive blending and motion trails
- No framework, no camera, no network permission required
