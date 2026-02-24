## 📂 Repository contents

* `README.md file`
* Description of tool
* How to print and assemble
* How to redesign


* `design_files/`
* `stl/` → ready-to-print STL files
* `f3d/` → Fusion 360 editable files
* `step/` → STEP files for CAD interoperability


* `printing/`
* `gcode/` → tested gcode files for 3D printers
* `slicer_profiles/` → PrusaSlicer config (.3mf / .ini)
* `printing_settings.md` → detailed printing settings


* `docs/`
* `zebrafish-molds-application-note.pdf`
* `figures/`


* `LICENSE`

---

# Customizable FDM 3D-printed zebrafish embryo molds for live imaging

This repository provides design files, printing instructions, and documentation for 3D-printed molds for orienting zebrafish embryos. The molds are designed to ensure dorsal positioning of embryos during live imaging  between 50 hours post-fertilization (hpf) and 5 days post-fertilization (dpf).

Unlike previously published molds fabricated with stereolithography (SLA)–based 3D printing (e.g., Geng & Peterson, 2021; Kleinhans & Lecaudey, 2019; Miller et al., 2025; Wittbrodt et al., 2014), our approach uses fused deposition modeling (FDM). Both SLA and FDM are part of the broader category of additive manufacturing, in which objects are built up layer by layer rather than removed from a solid block (subtractive manufacturing) or formed in a mold (injection molding).

* SLA printing relies on a laser or UV light to cure liquid resin layer by layer, producing parts with very fine resolution and smooth surfaces.
* FDM printing extrudes melted thermoplastic filament (such as PLA) through a heated nozzle to build up layers, making it widely accessible and cost-effective, but with lower resolution.

Because of these differences, SLA prints can reproduce the sharp triangular cavities of the CAD design, while FDM prints approximate them with rectangular cavities due to nozzle width (**Figure 1A** vs **1B**). Nevertheless, the molds (**Figure 2**) remain highly effective for stabilizing zebrafish embryos, while being affordable and easy to reproduce in most laboratory settings.

<p align="center">
<img src="docs/figures/FDMvsSLA.png" alt="FDM vs SLA printing comparison" width="600"/>
</p>

**Figure 1.** Differences, through g-code preview, in mold slots between FDM (**A**) and SLA (**B**) printing.

<p align="center">
<img src="docs/figures/Figure1_printing.png" alt="Zebrafish molds 3D designs" width="600"/>
</p>

**Figure 2.** FDM-printing-based mold design improves live in vivo imaging of brain vascularization in developing zebrafish embryos.
(**A**) CAD renderings of two circular mold sizes (20 mm and 13 mm) with slot dimensions in millimeters. Each slot measures 0.40 mm wide at the narrowest point, 0.60 mm at the widest, and extends 5.50 mm deep; the spacing between slots is 1.00 mm, and the slot height above the base is 2.00 mm. The smaller mold was designed for use with 14 mm coverslips, while the larger one was tested with 21 mm coverslips. The mold design was kept circular rather than rectangular to fit tightly within the well and stay level. Design files for both sizes are available for download via the associated GitHub repository.
(**B**) Perspective views of the assembled molds.
(**C**) Wells in 1.5% low-melting-point agarose were made using the seven- and twenty-tooth molds in 14- and 21-mm glass-bottom dishes, respectively.
(**D**) PrusaSlicer g-code preview illustrating how FDM resolution (0.4 mm nozzle) converts triangular cavities into rectangular slots.
(**E**) Exploded view of mold components, with a removable handle to facilitate positioning in small dishes.

<p align="center">
<img src="docs/figures/Figure2_liveimaging.png" alt="Zebrafish molds 3D designs" width="600"/>
</p>

**Figure 3.** FDM-printing-based mold design enables consistent live imaging of microglia motility and brain vascularization in developing zebrafish larvae.
(**A**) Top left: image showing empty agarose wells created using the seven-teeth mold. Bottom left: image showing 56 hpf *Tg(fli1a:GFP-CAAX)*; *Tg(gata1a:DsRed)* larvae inserted into the wells. The black-dotted box indicates the area magnified in the next panel. Right: magnified area of mounted larvae. Live brightfield imaging of the middle larvae, marked with an orange box, is presented in **panel G**. Scale bars: left panels 1 mm, right panel 500 µm.
(**B**) Brightfield midplane-volume image of the 56hpf *Tg(fli1a:GFP-CAAX)*; *Tg(gata1a:DsRed)* larvae from **panel F** (orange boxed region), before the start of time-lapse acquisition, shown in **panels H-I**, orange box. Scale bar: 50 µm.
(**C**) Maximum intensity projection of horizontal sections from overnight time-lapse imaging of vasculature, *Tg(fli1a:GFP-CAAX)* (cyan), and erythrocytes, *Tg(gata1a:DsRed)* (red), in the developing brain of the mounted larvae (identical to those shown in **panels F-G**, orange box). The first timepoint is shown in **panel (i)**. Temporal color coding of the *fli1:GFP* signal over the acquisition (time-lapse, 20-minute imaging interval, 32 time points) **(ii)**. The color bar indicates the transition from time point 1 (magenta) to 32 (bright yellow). See also Movie S1. Scale bars: 50 µm.
(**D**) High-magnification (63x) imaging of the brain vascularization process. The maximum intensity projection of the first acquisition time point is shown in **(i)**. The magnified area (indicated with an orange rectangle) shows filopodia-like protrusions extending from the *fli1:GFP*-positive (cyan) endothelial tip cell **(ii)**. The *gata1a:DsRed* positive erythrocytes (red) inside a more mature blood vessel are also shown. See also Movie S1. Scale bars: 25 µm and 5 µm, respectively.
(<p align="center">

<img src="docs/figures/Figure1_printing.png" alt="Zebrafish molds 3D designs" width="600"/>

</p>

) Temporal color coding of microglia dynamics in *Tg(mpeg1.1:GFP-CAAX)* 72 hpf larvae, over the acquisition period (10-minute imaging interval, 80 time points). The color bar indicates the transition from time point 1 (magenta) to 80 (bright yellow). Scale bar: 50 µm.
(**E**) Selected time-points from **panel E** (blue box),  showing microglia *Tg(mpeg1:GFP-CAAX)* (grey) migration and process elongation. Scale bar: 20 µm.

<p align="center">
<img src="docs/figures/MovieS1.gif" alt="Supplementary movie" width="600"/>
</p>

**Supplementary Movie S1.** Movie S1. Brain vascularization in the developing brain of a mounted larva. Development of brain vasculature and erythrocyte flow in more mature vessels was imaged in larvae expressing both *Tg(fli1a:GFP-CAAX)* (cyan) and *Tg(gata1a:DsRed)* (red) reporters. For **parts A** and **B**, the time intervals are 20 and 2 minutes, and the scale bars are 40 µm and 20 µm, respectively. For **part A**, acquisition was started at 54 hpf, and for **part B**, at 68 hpf (in the same larvae).

<p align="center">
<img src="docs/figures/MovieS2.gif" alt="Supplementary movie" width="600"/>
</p>

**Supplementary Movie S2.** Microglia migration and process extension dynamics in the developing brain of a mounted larva. Single microglia migration and elongation and retraction of its processes, labelled by *Tg(fmpeg1.1:GFP-CAAX)* (grey) reporter, was imaged for 12 hours. Time interval 10 minutes. Acquisition started at 72 hpf.  Scale bar 10  µm.

---

## 🔍 Design considerations

* **Circular footprint**: Chosen to fit tightly into 14 mm and 21 mm coverslip dishes.
* **FDM vs SLA**: FDM printing with a 0.4 mm nozzle limits precision, resulting in rectangular cavities instead of sharp triangular ones. Functionality is unaffected, but geometric fidelity is reduced.
* **Stage compatibility**: Optimized for zebrafish between 50 hpf–5 dpf.
* **Accessibility**: All files are openly shared for reproduction and adaptation.

⚠️ **Note:** Embryos younger than 50 hpf are too small for this design. Separate molds with smaller wells would be required. (see the [how-to/](how-to/README.md) folder).

## 📚 References

* Geng, Y., & Peterson, R. T. (2021). Rapid Mounting of Zebrafish Larvae for Brain Imaging. Zebrafish, 18(6), 376. https://doi.org/10.1089/zeb.2021.0062
* Kleinhans, D. S., & Lecaudey, V. (2019). Standardized mounting method of (zebrafish) embryos using a 3D-printed stamp for high-content, semi-automated confocal imaging. BMC Biotechnology, 19(1), 68. https://doi.org/10.1186/s12896-019-0558-y
* Miller, J. C., Koirala, P., Torre, M. F. A. de la, Farsi, M., Lieberth, J., Shrestha, R., & Bloomekatz, J. (2025). Custom 3D-Printed Molds for Zebrafish Imaging and Cardiac Development. Journal of Visualized Experiments (JoVE), 222, e68768. https://doi.org/10.3791/68768
* Wittbrodt, J. N., Liebel, U., & Gehrig, J. (2014). Generation of orientation tools for automated zebrafish screening assays using desktop 3D printing. BMC Biotechnology, 14(1), 36. https://doi.org/10.1186/1472-6750-14-36

---

## 📖 Citation

If you use these zebrafish molds in your research, please cite:

**Customizable FDM-based zebrafish embryo mold for live imaging** Rivera Pineda MX, Lehtimäki J, Jacquemet G.

*bioRxiv* (2025)
[](https://doi.org/10.1101/2025.11.24.689779)

