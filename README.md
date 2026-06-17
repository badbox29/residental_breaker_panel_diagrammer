# RPanel — Residential Breaker Panel Diagrammer

A homeowner-focused documentation tool for mapping and maintaining residential electrical panels.

RPanel helps you build a clean, visual representation of your breaker box so you always know what each circuit controls. Document rooms, appliances, amperage, breaker protection types, and panel metadata, then print or export a polished reference you can hang inside the panel door.

Everything runs entirely in a single HTML file — no accounts, no server, no build tools, and no installation required.

#### Demo

https://badbox29.github.io/residential_breaker_panel_diagrammer/

---

#### Screenshot

![Screenshot](screenshot.png)

---

## Features

### Panel Design

* **Interactive breaker panel editor** — click any slot to create, edit, or remove breakers
* **Realistic panel layout** — left/right numbered breaker positions modeled after residential load centers
* **Expandable panel size** — add or remove rows to match your actual panel configuration
* **Locked row removal** — rows can only be removed when both breaker positions are empty
* **Spare breaker support** — distinguish intentionally unused slots from truly empty ones

---

### Breaker Management

#### Breaker Types

* Standard
* GFCI
* AFCI
* Double-Pole (2-pole)

#### 2-Pole Breaker Intelligence

* Automatically links adjacent breaker positions
* Secondary slots are protected from accidental edits
* Removing either side cleans up the entire pair

#### Per-Breaker Details

Store information for every circuit.

* Circuit label
* Amperage
* Room / location
* Notes

#### Visual Type Badges

Breaker protection types are easy to identify at a glance.

---

### Header & Panel Metadata

Document important panel information directly on the diagram.

#### Header Fields

* Service address
* Install date
* Panel location

#### Footer Fields

* Manufacturer
* Model number
* Main panel rating
* Voltage
* Installer
* Additional notes

---

### Preset System

Build reusable panel templates.

* Save current panel as a named preset
* Load existing presets
* Update existing presets
* Delete unwanted presets
* Dedicated preset manager
* Presets are stored locally in your browser

Useful for:

* Similar homes
* Rental properties
* Family members
* Electricians documenting multiple panels

---

### Undo / Redo

Full editing history support.

* Undo (`Ctrl+Z`)
* Redo (`Ctrl+Y`)
* 20-step history stack

---

### Save & Recovery

#### Browser Save

* Save directly to local browser storage
* One-click restore
* Separate delete-saved function
* Theme preference persistence

#### JSON Export / Import

* Portable backup files
* Full panel restoration
* Schema validation
* Overwrite protection

#### Legacy File Migration

Older RPanel exports are automatically detected and upgraded.

Migration support includes:

* Legacy version detection
* Upgrade summaries
* Preset migration support
* Guided upgrade dialog

---

### Export Options

#### Print

Optimized printable output.

* Dedicated print stylesheet
* Automatically forces light mode
* Removes editing controls
* Preserves breaker colors
* Includes legend

#### PNG Export

Generate a high-resolution image.

* 4× rendering resolution
* Includes legend
* Optimized for sharing and documentation

---

### Interface Features

* Dark mode / light mode toggle
* Responsive toolbar
* Inline SVG icons
* Embedded application icon
* Modern confirmation dialogs
* Toast notifications throughout the application

---

## Setup

No setup required.

Download `index.html` and open it in any modern browser.

For a permanent URL, deploy it to GitHub Pages or any static host.

---

## Data & Privacy

All data stays on your computer.

* No accounts
* No cloud sync
* No telemetry
* No backend
* No tracking

Data is stored locally in your browser using `localStorage`.

External dependency:

* `html2canvas` (PNG export)

---

## Keyboard Shortcuts

| Shortcut | Action          |
| -------- | --------------- |
| `Ctrl+S` | Save to browser |
| `Ctrl+Z` | Undo            |
| `Ctrl+Y` | Redo            |

---

## File Structure

```text
residential_breaker_panel_diagrammer/
├── index.html
├── screenshot.png
├── README.md
└── LICENSE
```

---

## License

See LICENSE file.
