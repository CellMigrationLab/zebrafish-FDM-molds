# How-to guides

This directory contains how-to guides related to the FDM-printed zebrafish embryo orientation molds.  

## 📂 Content
- **how-to 1: redesign the wells** → Modify the molds according to the developmental stage of your zebrafish embryos/larvae.
- **how-to 2: print and assemble** → Print and assemble your molds.


  
## How-to 1: Redesign the wells

***Note 1:*** Changing one dimension of the first well propagates to the others. Therefore, after edits, you should always check for overlapping and spacing. 
***Note 2:*** These steps can be implemented to modify other dimensions of the mold, such as the depth of the wells or diameter of the mold.
***Note 3:*** All redesign steps were performed in Autodesk Fusion 360. Although Fusion 360 is subscription-based, a free educational license is available for academic users.

Steps:
1. Open the corresponding mold file (.f3d file) in Fusion 360. Open the wells sketch by double-clicking the first sketch in the Timeline (highlighted by the red rectangle in Figure 3A).
2. Modify well dimensions by double-clicking the desired dimension as shown in Figure 3B (red rectangle). Edit the relevant dimensions (head width, neck width, length) according to the embryo/larvae stage. See Figure 3E for suggested dimensions based on embryo stage (based on Kimmel et al. (1995)).
3. After resizing the wells, check the dimension regarding the distance between the first well and the edge reference. Update it so the modified wells still fit cleanly within the diameter boundary. E.g.: 1.4 mm (Figure 3B, red triangle) to 1.2 mm (Figure 3C, red triangle) after changing the well geometry.
4. Verify spacing and pattern integrity by ensuring that the wells don’t overlap after the update. If the wells overlap, modify the spacing by zooming in, and double clicking the Rectangular Pattern Constraint (dotted rectangle in Figure 3D) and adjusting the amount of wells (green triangle in Figure 3D) and distance between them (magenta triangle in Figure 3D).
5. Click Finish Sketch. In the Timeline, confirm the extrude and cut features regenerated correctly.
6. Export the updated mold as an STL file and proceed to slicing and 3D printing. To export, go to File> Export…, and change the Type to STL Files (*.stl).

<p align="center">
<img src="../docs/figures/Figure3. how-to-redesign.png" alt="how to redesign the zebrafish molds" width="900"/>
</p>

**Figure 1.** How to redesign the zebrafish molds. 
(A) Autodesk Fusion 360 project file showing the mold with replicated wells arranged to fit a standard glass-bottom imaging dish. The red rectangle highlights the sketch to edit to modify the wells’ dimensions.
(B–C) The well sketch can be edited by opening the first sketch in the Timeline and modifying the parameterized dimensions (example shown for the first well; red rectangle). After resizing, the offset between the first well and the dish boundary should be updated to ensure the pattern remains within the circular mold footprint (red triangle). 
(D) If resizing causes wells to overlap, spacing and/or the number of wells can be adjusted using the Rectangular Pattern Constraint (dotted black rectangle). 
(E) Suggested stage-dependent dimensions to guide redesign: (Ei) embryo measurements (dorso- ventral orientation) extracted from Kimmel et al. (1995); (Eii) corresponding recommended well parameters for FDM printing; (Eiii) corresponding parameters for higher-precision printing (e.g., SLA). Right: schematic of the well geometry indicating the editable parameters A-D (mm) used throughout the tables.

---

## 🖨 How-to 2: Printing and assembly instructions

1. Download STL files from `design_files/stl/`.
2. Open in PrusaSlicer (or your slicer of choice).  
   - Recommended settings are included in `printing/printing_settings.md`.
3. Print using PLA material with a 0.4 mm nozzle.  
4. ⚠️ Critical step.  To minimize adhesion to the agarose gel, sand the printed molds carefully but roughly. This will increase surface porosity for resin infiltration (next step). 
5. Apply a thin coat of two-part epoxy over all surfaces of the mold that contact the agarose gel to create a smooth, sealed surface. Allow to cure fully before use (24h or as required by the manufacturer).
6. The stamp component is glued to the middle ring, forming a single object and creating an internal pocket. 
7. The stem is inserted into this pocket and rotated ~180° to lock or unlock its position. Once assembled, the mold is ready for use.

<p align="center">
<img src="../docs/figures/Figure4_assembly_zebrafish_molds.png" alt="zebrafish mold assembly steps" width="600"/>
</p>

**Figure 2.** Assembly of the zebrafish molds.



