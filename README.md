# Pixelmap — LED Pixelmap Generator

A browser tool to lay out, document and export **LED screens (pixelmaps)** and
**test patterns**. Everything runs locally in your browser — no server required,
and your data stays on your own machine.

- **Live:** https://genes-media.nl
- **Tech:** a single `index.html` (HTML/CSS/JS, no build step). GitHub Pages
  publishes automatically on every push to `main`.

---

## Contents

- [Quick start](#quick-start)
- [Two modes](#two-modes)
- [Canvas navigation](#canvas-navigation)
- [Managing screens](#managing-screens)
- [Screen properties](#screen-properties)
  - [Grid mode](#grid-mode)
  - [Advanced mode (free tile placement)](#advanced-mode-free-tile-placement)
  - [Enlarged tile editor](#enlarged-tile-editor)
  - [Per-screen overlays](#per-screen-overlays)
- [Project & Projects](#project--projects)
- [Overlays](#overlays)
- [Display options](#display-options)
- [Presets](#presets)
- [Exporting](#exporting)
- [Test patterns](#test-patterns)
- [Keyboard & mouse shortcuts](#keyboard--mouse-shortcuts)
- [Storage & back-up](#storage--back-up)

---

## Quick start

1. Open https://genes-media.nl
2. Your **screens** are on the left, the **canvas** (preview) in the middle, and
   the **settings** on the right.
3. Set the canvas size and title under **Project** (top right).
4. Select a screen on the left and configure it under **Screen properties**.
5. Done? Click **Download PNG** (top right).

Switch language with **EN / NL** (top right); toggle light/dark with the
sun/moon icon.

---

## Two modes

Switch at the top between:

- **Pixelmap** — arrange your LED screens on a canvas (the main mode).
- **Test patterns** — generate test images (colour bars, grayscale ramps, grids,
  etc.) at a chosen resolution.

---

## Canvas navigation

In both the pixelmap and the test-pattern preview:

- **Zoom in/out:** scroll the mouse wheel — it zooms toward the **cursor
  position**.
- **Pan:** hold the **middle mouse button** and drag.
- **Zoom level:** the **Fit / 50% / 100% / 200%** buttons below the preview.
- Live **VIEW / CURSOR / TILE** info sits in the bottom-left corner.

---

## Managing screens

In the left column (**Screens**):

- **+** (top right) adds a screen.
- Click a screen to select and edit it.
- **Double-click** the name to rename it.
- **×** removes a screen.

On the canvas each screen shows its **0,0 position** in the **top-left corner**
(the canvas pixel coordinate of that corner). The value updates live while you
drag a screen, and can be toggled off under *Display options → Screen 0,0
position*.

---

## Screen properties

At the top of this panel you choose **Grid mode** or **Advanced** per screen.

### Grid mode

A regular grid of identical tiles:

- **Tile pixels** — width × height of one tile (in pixels).
- **Grid (cols × rows)** — number of columns and rows.
- **Offset** — the screen's position on the canvas (x, y).
- **Colors** — colour A and B (checker/gradient).
- **Gradient** — Checker (A+B), gradient per tile, or gradient across the whole
  screen, with a direction.
- **Rebuild this screen's grid** — rebuilds the grid.

Turn individual tiles on/off with the **tile tool** (click/drag on the canvas).

### Advanced mode (free tile placement)

For irregular walls: define one or more **tile types** (each with its own size
and colours) and place them freely:

- **+ Add tile type** — a new tile type.
- Select a type, click the editor canvas to place; drag to move; **right-click**
  or **Delete** to remove.
- **Snap** — place on a grid (adjustable step size).
- **Clear all** — remove all placed tiles.

### Enlarged tile editor

The advanced editor canvas is small; click **⤢ Enlarge** to open it **temporarily
in a large window**. In that window:

- **Zoom** with the mouse wheel (toward the cursor) and **pan** with the middle
  mouse button.
- **Fit view** (top right) resets the view to fit.
- The **tile-type picker, snap and Clear all** live in the left sidebar, so you
  can pick/add tiles without closing.
- Close with **✕**, **Escape**, or a click outside the window. Everything returns
  to the side panel.

### Per-screen overlays

At the bottom of Screen properties, per screen:

- **Circle** and **Cross** — circle and diagonal-cross overlays (on by default,
  white, 2px).
- **Color** and **Line width** — colour and line width of those overlays.
- **Screen info overlay** — a draggable/resizable info box with the screen name,
  project name and resolution. On by default for a new project, and it moves
  along when you drag the screen.

---

## Project & Projects

The **Project** card (top right) contains:

- **Title / Subtitle** — title and subtitle (also used by the "Project info"
  overlay).
- **Canvas** — the total canvas size in pixels.
- **Accent color** — colour for outlines, overlays and labels.
- **Canvas background** — background colour (with White/Black shortcuts).

Below it (**Projects**) you manage whole shows:

- **+ New project** — save the current setup as a new project.
- **Save** — update the active project.
- **Import project JSON** — load a previously exported project.

Projects are stored in your browser; export to JSON to back up or move to another
machine.

---

## Overlays

Add items that sit on top of the canvas (drag to place, drag the corners to
resize):

- **+ Color bar** — a colour bar.
- **+ Grayscale** — a grayscale ramp.
- **+ Project info** — title + subtitle + resolution.
- **+ Add logo** — your own image (PNG/JPG/GIF/SVG/WebP).

---

## Display options

Toggles for what is drawn on the canvas, including:

- **Tile coordinates** — per-tile coordinates.
- **Grid lines between tiles** — grid lines between tiles (on by default).
- **Inactive tile hints** — hints for inactive tiles.
- **Dimension rulers** — rulers showing the total size in px.
- **Title + spec table** — title block with a specification table.
- **Per-screen outline** — accent border around each screen.
- **Canvas corner coords** — the canvas corner coordinates.
- **Screen 0,0 position** — the canvas pixel position of each screen's 0,0 corner.
- **Canvas dimension labels** — canvas size labels.
- **Center text on screens** — text in the centre of screens (with adjustable
  size).

---

## Presets

Quickly load or store settings:

- Built-in presets plus your own **Save current**.
- **Export JSON / Import JSON** for exchange.

---

## Exporting

- **Download PNG** (top right) exports the canvas as an image.
- If the title + spec table don't fit on one page, the message *"Info doesn't fit
  on page 1"* appears at the top and a **second page** is added on download. Use
  **◀ 1 / 2 ▶** to page through the preview.

---

## Test patterns

In **Test patterns** mode:

1. Pick a **pattern** on the left (colour bars, grayscale, grid, crosshatch, …).
2. Set the **resolution** on the right (presets or custom) and the pattern
   options.
3. **Render** and export.

Use **↻ From pixelmap** to take over the screen layout from the pixelmap mode.

---

## Keyboard & mouse shortcuts

| Action | Shortcut |
|--------|----------|
| Zoom in/out (toward cursor) | Mouse wheel |
| Pan | Middle-mouse drag |
| Move a screen | **Alt + click** drag (or the move/grab tool) |
| Delete a tile (advanced) | Right-click or **Delete** |
| Close the enlarged editor | **Escape** |

---

## Storage & back-up

Projects, presets and settings are saved in your **browser's localStorage**. That
means:

- They are tied to this browser on this device.
- Clearing your browser data removes them.

👉 So export important projects to **JSON** as a back-up, or to use them on
another device.
