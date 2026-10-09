# Design-file guide

This project originated from mixed folders with unusual path characters. The files have been grouped by engineering subsystem and format without modifying the source design bytes.

## CAD

| Folder | Description | Open with |
| --- | --- | --- |
| `cad/turbo-adapters/freecad/` | Native turbo-adapter design sources | FreeCAD |
| `cad/turbo-adapters/step/` | Manufacturable/neutral geometry exports | FreeCAD or other STEP-capable CAD |
| `cad/turbo-adapters/stl/` | Mesh exports for preview or prototyping | Any STL viewer |
| `cad/transmission-actuation/` | Servo horn, servo bracket, bearing-related CAD and exports | FreeCAD / STEP / STL viewers |
| `cad/legacy-unlabeled/` | Original `Unnamed1` and `Unnamed2` projects and models; purpose not inferred | FreeCAD / STL viewer |

Some filenames contain original typographical errors such as `adapater` or `Guage`. They were intentionally **not renamed**, to preserve your design-file naming and internal references.

## Electronics

- `electronics/schematic/`: editable KiCad `.kicad_sch` file.
- `electronics/manufacturing/gerbers/solenoid-control/`: fabrication layers plus plated/non-plated drill files.
- No `.kicad_pcb` was found in the supplied archive. The Gerbers cannot replace the editable layout.

## Other files

- `docs/original-development-log.md` preserves original dated revision notes.
- `assets/previews/` contains images generated directly from supplied STL models, not photographs of completed hardware.
- Local FreeCAD `.FCBak` backups, duplicate Gerber copies, third-party reference drawings/photos, and the old TCU README are in a **separate offline-only package** and intentionally excluded from the public repo.

**Before manufacturing:** verify dimensions, clearances, materials, fastener specifications, load paths, and drawing revisions. Native models and exported meshes may not be synchronized.
