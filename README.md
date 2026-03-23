# Game of Life

A browser-based implementation of Conway's Game of Life with an interactive editor. Just open the HTML file — no build tools or dependencies required.

## Features

- **Infinite board** using a sparse Set (only living cells are stored)
- **Draw tool** — click to toggle cells, drag to draw/erase
- **Select tool** — drag to select a region of cells
- **Pan tool** — drag to move the viewport
- **Move tool** — drag a selection to reposition cells on the board
- **Mouse shortcuts** — middle-click to pan, right-click to select (regardless of active tool)
- **Zoom** — scroll wheel, centered on cursor
- **Simulation controls** — Step, Play/Pause, adjustable speed (0.2–20 gen/s)
- **Show Next** — preview the next generation with color overlays (blue = birth, red = death)
- **Undo/Redo** — up to 100 states of history
- **Cut/Copy/Paste** — works with selected regions; paste auto-selects the Move tool
- **Keyboard shortcuts** — Ctrl+C, Ctrl+V, Ctrl+X, Ctrl+Z, Ctrl+Y, Space (play/pause)
- **Import/Export** — save and load full board state as CSV
- **Save/Load Sections** — save a selection to CSV, load a section file into the clipboard for pasting

## Included Patterns

The repo includes a library of classic Game of Life patterns as CSV files, organized by category:

| Category | Patterns |
|---|---|
| **Static** (still lifes) | block, boat (NE/NW/SE/SW), hive (horizontal/vertical), loaf, tub, lopsided o, acorn end state |
| **Oscillators** | blinker, toad, beacon, pulsar, pentadecathlon |
| **Spaceships** | glider (NE/NW/SE/SW), glider crash (4-way), LWSS, MWSS, HWSS (E/N), c/10 orthogonal, hammerhead |
| **Methuselahs** | r-pentomino (1103 gen), diehard (130 gen), acorn (5206 gen), figure eight (250 gen) |
| **Generators** | Gosper glider gun, max spacefiller |
| **Fillers** | netmaker |

Use **Load Section** in the sidebar to load any pattern into the clipboard, then **Paste** to place it on the board.

## Usage

Open `game_of_life.html` in any modern browser.

## CSV Format

Board and section files use a simple CSV format:

```
# Comment lines start with #
x,y
x,y
...
```

Each line is the coordinate of a living cell. Section files use coordinates relative to the top-left of the selection.
