# Conway's Game of Life

As someone deeply fascinated by AI and complex systems, I built this project out of curiosity for how simple rules can give rise to surprisingly complex behaviour. Conway's Game of Life felt like the perfect starting point to explore the intersection of simulation, emergent patterns, and computational thinking


A fully interactive, browser-based simulation of **Conway's Game of Life** — a classic cellular automaton invented by mathematician John Horton Conway in 1970.

![Game of Life Preview](https://img.shields.io/badge/HTML5-Canvas-orange?style=flat-square&logo=html5)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![No dependencies](https://img.shields.io/badge/dependencies-none-brightgreen?style=flat-square)

## ✨ Features

- **Interactive grid editor** — click or drag cells to toggle alive/dead states
- **Three draw modes** — Toggle, Set Alive, Set Dead
- **Run / Pause / Step** simulation controls
- **Adjustable speed** — 1 to 60 generations per second
- **Configurable grid size** — up to 500 × 500 cells
- **8 built-in patterns** — Glider, Blinker, Toad, Beacon, Pulsar, R-Pentomino, Gosper Glider Gun, Random
- **Live statistics** — generation count, alive cells, population %, born/died per step
- **Dark & Light mode** with system preference detection
- **Keyboard shortcuts** — `Space` run/pause, `→` or `n` step, `c` clear
- **Touch support** for mobile and tablet
- **Zero dependencies** — pure HTML + CSS + JavaScript

## 🚀 Quick Start

### Option 1: Open directly in browser

Just open `index.html` in any modern browser — no server needed.

```bash
open index.html          # macOS
xdg-open index.html      # Linux
start index.html         # Windows
```

### Option 2: Serve locally

```bash
# Python 3
python3 -m http.server 8080

# Node.js (npx)
npx serve .

# Then open http://localhost:8080
```

### Option 3: GitHub Pages

Push this repository to GitHub and enable **GitHub Pages** (Settings → Pages → Deploy from branch `main`, root `/`). Your simulation will be live at:

```
https://<your-username>.github.io/conways-game-of-life/
```

## 🎮 Usage

### Controls

| Control | Action |
|---|---|
| **Run / Pause** button | Start or stop the simulation |
| **Step** button (⏭) | Advance one generation at a time |
| **Clear** button 🗑️ | Clear the entire grid |
| **Speed slider** | Set simulation speed (1–60 gen/s) |
| **Grid size inputs** | Change columns & rows, then click *Apply Grid Size* |

### Draw Modes

| Mode | Behavior |
|---|---|
| **Toggle** | Click/drag flips each cell's state |
| **Set Alive** | Drag to paint living cells |
| **Set Dead** | Drag to erase cells |

### Keyboard Shortcuts

| Key | Action |
|---|---|
| `Space` | Run / Pause |
| `→` or `n` | Step one generation |
| `c` | Clear grid |

### Patterns

Click any pattern button in the sidebar to stamp it into the center of the grid:

- **Glider** — travels diagonally across the grid
- **Blinker** — oscillates between two states (period 2)
- **Toad** — period-2 oscillator
- **Beacon** — period-2 oscillator
- **Pulsar** — large period-3 oscillator
- **R-Pentomino** — small shape with a long, chaotic evolution
- **Glider Gun** — Gosper Glider Gun, endlessly spawns gliders
- **Random** — fills grid with ~30% random live cells

## 📐 The Rules of Conway's Game of Life

Each cell is either **alive** (1) or **dead** (0). At each generation, every cell is updated simultaneously based on its 8 neighbours:

1. A **live cell** with 2 or 3 neighbours **survives**
2. A **dead cell** with exactly 3 neighbours becomes **alive** (reproduction)
3. All other live cells **die** (under-population or over-population)
4. All other dead cells **stay dead**

## 🏗️ Project Structure

```
conways-game-of-life/
├── index.html       ← Complete app (HTML + CSS + JS, single file)
├── README.md        ← This file
├── LICENSE          ← MIT License
└── .gitignore       ← Git ignore rules
```

The entire application is a **single self-contained HTML file** with no external dependencies beyond Google Fonts (loaded via CDN). It works fully offline if fonts fall back to system fonts.

## 🌐 Browser Compatibility

| Browser | Support |
|---|---|
| Chrome / Edge 90+ | ✅ Full |
| Firefox 89+ | ✅ Full |
| Safari 15+ | ✅ Full |
| Mobile Chrome/Safari | ✅ Touch supported |

## 📜 License

MIT — see [LICENSE](LICENSE).

---

*Built as a cellular automata exercise. Dedicated to John Horton Conway (1937–2020).*
