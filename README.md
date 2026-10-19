# Home planner

An interactive 3D home-layout planner built with HTML, CSS, JavaScript, and Three.js. It helps explore furniture arrangements against room measurements before purchasing furniture. The first room is a kitchen dining nook, modeled from a reference photo and measurements, with an Article Rosin banquette and adjustable dining tables.

## Features

- Orbitable 3D scene with neutral, shadow-free lighting and photo-inspired materials.
- Six Rosin footprints: long/short corner, long/short L, straight long, and U; flip the return between wall and kitchen sides.
- Plank+Beam Risa comparison preset with wood back and cream cushions, provisionally using its dimension drawing (64.75 × 63 inches); conflicting written specifications are flagged.
- Independent visibility controls for the table, Rosin and opposite seating; larger Rosin footprints flag measured-span overruns.
- Top-down floor plan with draggable table placement.
- Adjustable table size, rotation, base and room spans.
- Round, extendable oval and rectangular table presets.
- Switch between opposite chairs, a bench or no extra seating.
- Live edge-clearance calculations and optional diner markers.
- Browser autosave plus JSON layout export/import.

## Quick start

Download or clone this repository and open `kitchen-planner.html` in a modern browser. No build step, package installation, backend or account is required. An internet connection is needed for the pinned Three.js CDN dependency.

Alternatively, run `python3 -m http.server 8000` from the repository folder and visit `http://localhost:8000/kitchen-planner.html`. In Codex, open that URL or the local HTML file in the browser side panel.

## Accuracy and privacy

This is a planning prototype, not architectural CAD or a photogrammetric reconstruction. Measured dimensions and estimates are documented in `ROOMS.md`. Clearances and diner markers do not certify fit, comfort or seating capacity. Verify product specifications and on-site measurements before purchasing.

Room dimensions and descriptions are included in this repository; original photos and exported personal layout files are not. Layout state remains in browser storage or a user-downloaded JSON file. The app loads Three.js from jsDelivr but has no application backend or analytics.

Open `kitchen-planner.html` in a browser or the Codex side panel. It is a standalone editable planner, not an installed plugin. It requires internet access to load Three.js from jsDelivr; no local server is required.

## Returning to this project

Open this folder as a local project in Codex, or give Codex this folder path and ask to continue the home planner. Start with `ROOMS.md` for the verified room context and remaining measurement questions.

The kitchen supports orbiting, a draggable floor plan, table dimensions and rotation, Rosin seating, alternative table bases, a bench or chairs, and optional diner markers. Use **Save layout to file** to download your exact settings. Use **Load saved layout** to restore them. Browser autosave is convenient but does not necessarily transfer between local-file and localhost previews or other browsers.

## Adding another room

Ask Codex to add the room using its photos and measurements, preserving the kitchen. Keep one room entry in `ROOMS.md` and a separate room implementation until a shared room selector is built. The current app only models the kitchen; multi-room switching is future work.

## Files

- `kitchen-planner.html`: application and editable source.
- `ROOMS.md`: room evidence, orientation, measurements, uncertainties.
- `AGENTS.md`: instructions for future development.

The original Notes photos are not bundled. One kitchen photo was inspected in Apple Notes → House measurements. Future work requiring exact photographic detail should reopen that note or use additional photos supplied by the user.
