# DraftBench release notes

Website: https://dwg.jskrnh.xyz

## v1.2
- **Fix: DWG files are now selectable and editable.** Layer lock and frozen flags were read wrongly, so every layer opened locked. They now come from the file's real flags, and clicking an object on a genuinely locked layer tells you why.
- **Drawing tabs.** Open several DWG/DXF files at once (Open accepts multiple files, or drop them on the canvas). Each tab keeps its own undo history, view and unsaved-changes marker. Close with ×, or middle-click; closing unsaved work asks you to click twice.
- **Layer Manager** (Layers button, or LA). Table of every layer with visibility, lock, color picker, linetype, object count and rename. Multi-select with Ctrl/Shift, then New, Delete (moves objects to a layer you choose), Set current, Isolate, Show all, Unlock all, Select objects on layer, Purge empty, Move selected objects here, and a filter box.
- New commands: LAYISO, LAYON, LAYOFF, LAYLCK, LAYULK, UNLOCKALL, LAYMCUR.
- Copy and paste between tabs (Ctrl+C, Ctrl+V; COPYCLIP, PASTECLIP). Blocks and layers come along.

## v1.1
- Standalone build for static hosting. DXF, SVG and PDF download directly as normal files.
- Deployed from GitHub to Cloudflare Pages.

## v1.0
- Opens DWG and DXF. Saves DXF (R12), exports SVG, plots PDF at scale.
- Draw, modify, dimension, hatch, blocks, layers, properties, object snaps, command line.
- DWG is read-only: saving always writes a DXF copy.
