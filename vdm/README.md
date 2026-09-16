# Digital Sculptor VDM Catalog

This directory hosts the default Vector Displacement Map brush catalog used by Digital Sculptor.

## Contents

- `manifest.json`: catalog metadata consumed by the app.
- `textures/`: 50 tangent-space VDM textures encoded as 8-bit RGBA PNG.
- `thumbnails/`: generated preview images.
- `credits.json`: source author, asset page, and license for every brush.

All 50 source brushes were selected from 226 CC0 BlenderKit brush assets
and verified inside Blender to have `use_color_as_displacement` enabled.
The catalog includes anatomy, skin detail, creature, rock, surface, and
ornament brushes. Every selected source asset is marked `CC0 1.0` by
BlenderKit. The original asset page and author are recorded per entry in
`credits.json`.

The source floating-point displacement is normalized into RGB around byte value 128. The original maximum absolute component is stored in each manifest entry as `metadata.scale`, allowing the app to reconstruct the source displacement range.
