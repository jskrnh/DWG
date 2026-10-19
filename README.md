# DraftBench

https://dwg.jskrnh.xyz

Browser-based 2D CAD. Opens DWG and DXF, draws and edits with AutoCAD-style commands, saves DXF, exports SVG, plots to PDF at scale.

## Hosting

Static site, no build step. Cloudflare Pages settings:

- Framework preset: None
- Build command: (empty)
- Build output directory: `/`

## Files

- `index.html`: the whole app (drafting core + UI)
- `libredwg.js`, `libredwg.wasm`: DWG reader, from `@mlightcad/libredwg-web` 0.6.6 (GPL-2.0-only)
- `_headers`: file type and caching rules for Cloudflare Pages

## License note

`libredwg.js` and `libredwg.wasm` come from libredwg-web, which is GPL-2.0-only. Keep this source available alongside the deployed site.
