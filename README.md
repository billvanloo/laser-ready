# laser-ready
A simple, lightning-fast utility for converting PDFs from Onshape so they are ready to laser cut using a ULS laser engraver.

To use the utility, just upload a PDF (or DXF) that contains line art. The utility will select all lines in the PDF, change them to the correct RBG color value of 255,0,0, then change the line width to 0.001 inches. A new PDF, named `LaserReady_<original name>.pdf` by default, will then be downloaded, which can be opened in Adobe Acrobat and sent to a ULS laser engraver for cutting.

## Input formats

- **PDF** — every stroke is recolored to 255,0,0 and every line width set to 0.001 inches.
- **DXF** — the drawing is redrawn as a PDF at true 1:1 scale (using the file's `$INSUNITS`; millimeters are assumed when units aren't set), on a page fitted to the geometry with a 0.25" margin. Lines, polylines (including arcs), circles, arcs, ellipses, splines and blocks are converted to red 0.001" cut lines. Dimensions, hatches and hidden/frozen layers are skipped.
  - **Engrave text:** tick *dxf text → engrave* to include TEXT/MTEXT as black filled text for raster engraving. Off by default.
- **DWG** — not supported, since DWG can't be read in the browser. In Onshape, export the drawing or sketch as DXF instead.

The output is always a PDF.

## Filename prefix

Output files are named `<prefix>_<original name>.pdf`. The prefix defaults to `LaserReady` and can be changed in the app (letters and numbers only); your choice is remembered in the browser.

This was built using Claude. Please don't use this tool if you have qualms about using code created with AI tools.

## Privacy

All processing happens in your browser. No file is ever uploaded to a server.

## Credits & support

- Designed by **Bill Van Loo**
- Found a bug or want a feature? Email `billvanloo.tech+feedback@gmail.com` (the subject line is pre-filled from the in-app links).
- If this tool saved you time, you can [support the work on Ko-fi](https://ko-fi.com/billvanloo).

## License

[MIT](LICENSE) © 2026 Bill Van Loo

