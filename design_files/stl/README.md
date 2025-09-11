# STL Files (`.stl`)

This folder contains the STL files for the zebrafish embryo molds. STL files describe the mesh geometry of the model and are the most common format for 3D printing. These are the files most users will want to download and slice directly.

## Files
- **`zfish-mold-stamp/stemlock/stem-D13.stl`** → Mold with 13 mm diameter, designed for 14 mm coverslip plates.  
- **`zfish-mold-stamp/stemlock/stem-D20.stl`** → Mold with 20 mm diameter, tested with 21 mm coverslip plates.  

## Notes
- STL files are ready-to-slice in PrusaSlicer, Cura, or other slicers.  
- Unlike `.f3d` or `.step` files, STLs do not include parametric history or editable sketches. They are mesh-only files intended for printing.  
- To modify geometry (e.g., slot width, spacing, or mold diameter), use the editable `.f3d` (Fusion 360) or `.step` files instead.  
- Both STL versions share the same slot dimensions:  
  - Slot depth: **5.50 mm**  
  - Narrow width: **0.40 mm**  
  - Wide width: **0.60 mm**  
  - Slot spacing: **1.00 mm**  
  - Slot height above base: **2.00 mm**  

## Recommended workflow
1. Choose the STL that matches your imaging dish (13 mm or 20 mm).  
2. Open in PrusaSlicer (or another slicer).  
3. Apply the provided print settings (`printing/printing_settings.md` or `.ini`/`.3mf` profile).  
4. Export G-code and print.  
