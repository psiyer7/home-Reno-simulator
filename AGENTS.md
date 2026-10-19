# Home planner development

Read README.md and ROOMS.md before changing room geometry.

Preserve user layout settings and all orientation corrections. Distinguish measured dimensions from photo estimates. Do not invent room dimensions or assert a seating capacity solely from the number of visible figures.

The app is a standalone Three.js HTML file. Keep it usable from a local file and the Codex browser side panel. It currently loads a pinned Three.js dependency from a CDN, so do not claim offline availability.

For additional rooms, preserve the kitchen and its state key. Give each room its own saved state and measurement record. Keep exported layout files versioned. Validate imports and never execute imported content.

After meaningful UI or geometry changes, inspect the 3D view and floor plan in the browser, exercise relevant controls, and preserve saved user settings. Explicitly disclose remaining measurement uncertainty.
