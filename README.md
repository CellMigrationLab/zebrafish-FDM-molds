# Customizable FDM 3D-printed zebrafish embryo molds for live imaging

This repository provides design files, printing instructions, and documentation for 3D-printed zebrafish embryo orientation molds. The molds are designed to ensure dorsal positioning of embryos during live imaging  between 48 hours post-fertilization (hpf) and 5 days post-fertilization (dpf).

Unlike previously published molds fabricated with stereolithography (SLA)–based 3D printing (e.g., Geng & Peterson, 2021; Kleinhans & Lecaudey, 2019; Miller et al., 2025; Wittbrodt et al., 2014), our approach uses fused deposition modeling (FDM). Both SLA and FDM are part of the broader category of additive manufacturing, in which objects are built up layer by layer rather than removed from a solid block (subtractive manufacturing) or formed in a mold (injection molding).
- SLA printing relies on a laser or UV light to cure liquid resin layer by layer, producing parts with very fine resolution and smooth surfaces.
- FDM printing extrudes melted thermoplastic filament (such as PLA) through a heated nozzle to build up layers, making it widely accessible and cost-effective but with lower resolution.

Because of these differences, FDM produces less precise cavity shapes (rectangular rather than the sharp triangular features of the original CAD design). Nevertheless, the molds remain highly effective for stabilizing zebrafish embryos, while being affordable and easy to reproduce in most laboratory settings.

---

## 📂 Repository contents

- `design_files/`
  - `stl/` → ready-to-print STL files  
  - `f3d/` → Fusion 360 editable files  
  - `step/` → STEP files for CAD interoperability  
- `printing/`
  - `gcode/` → tested gcode files for 3D printers  
  - `slicer_profiles/` → PrusaSlicer config (.3mf / .ini)  
  - `printing_settings.md` → detailed printing settings  
- `docs/`
  - `zebrafish-molds-application-note.pdf`  
  - `figures/`   
- `LICENSE`  

---

## 🖨 Printing instructions

1. Download STL files from `design_files/stl/`.
2. Open in PrusaSlicer (or your slicer of choice).  
   - Recommended settings are included in `printing/printing_settings.md`.
3. Print using PLA material with a 0.4 mm nozzle...  
4. Sand the printed molds to remove rough edges.  
5. Apply a thin coat of two-part epoxy to create a smooth, sealed surface. Allow to cure fully before use.

---

## 🧪 Usage (needs revision)

1. Pour 1% low-melting agarose into a 35 mm imaging dish.  
2. While still soft, press the mold into agarose to create embryo-shaped wells.  
3. Place zebrafish embryos (48 hpf-5 dpf) into the wells.  
4. Add E3 medium (optionally with tricaine for anesthesia).  
5. Proceed with imaging.  

⚠️ **Note:** Embryos younger than 48 hpf are too small for this design. Separate molds with smaller wells would be required.

---

## 🔍 Design considerations

- **Circular footprint**: Chosen to fit tightly into 14 mm and 21 mm coverslip dishes. 
- **FDM vs SLA**: FDM printing with a 0.4 mm nozzle limits precision, resulting in rectangular cavities instead of sharp triangular ones. Functionality is unaffected, but geometric fidelity is reduced.  
- **Stage compatibility**: Optimized for zebrafish between 48 hpf–5 dpf.  
- **Accessibility**: All files are openly shared for reproduction and adaptation.

## 📚 References

- Geng, Y., & Peterson, R. T. (2021). Rapid Mounting of Zebrafish Larvae for Brain Imaging. Zebrafish, 18(6), 376. https://doi.org/10.1089/zeb.2021.0062 
- Kleinhans, D. S., & Lecaudey, V. (2019). Standardized mounting method of (zebrafish) embryos using a 3D-printed stamp for high-content, semi-automated confocal imaging. BMC Biotechnology, 19(1), 68. https://doi.org/10.1186/s12896-019-0558-y 
- Miller, J. C., Koirala, P., Torre, M. F. A. de la, Farsi, M., Lieberth, J., Shrestha, R., & Bloomekatz, J. (2025). Custom 3D-Printed Molds for Zebrafish Imaging and Cardiac Development. Journal of Visualized Experiments (JoVE), 222, e68768. https://doi.org/10.3791/68768 
- Wittbrodt, J. N., Liebel, U., & Gehrig, J. (2014). Generation of orientation tools for automated zebrafish screening assays using desktop 3D printing. BMC Biotechnology, 14(1), 36. https://doi.org/10.1186/1472-6750-14-36 

---

## 📖 Citation


