# Automated fluorescence quantification of extracellular vesicles collected from blood plasma using dielectrophoresis

## Citation (NLM)
Gustafson KT, Huynh KT, Heineck D, Bueno J, Modestino A, Kim S, Gower A, Armstrong R, Schutt CE, Ibsen SD. Automated fluorescence quantification of extracellular vesicles collected from blood plasma using dielectrophoresis. Lab Chip. 2021;21:1318-1332. doi: 10.1039/d0lc00940g

**DOI:** [https://doi.org/10.1039/d0lc00940g](https://doi.org/10.1039/d0lc00940g)

---

## Background
- Tumor-secreted exosomes and extracellular vesicles (EVs) are valuable biomarkers for early cancer detection, but their small size (50-150 nm) and low buoyant density make recovery from blood challenging
- Conventional ultracentrifugation and filtration-based methods are time-consuming and labor-intensive
- DEP (dielectrophoresis)-based lab-on-a-chip enables efficient EV recovery from blood plasma
- Low biomarker concentrations in early-stage cancer patients require SNR improvement and background noise separation

## Key Experiment Methods
1. **DEP chip**: Circular electrode planar microarray, AC voltage creates non-uniform electric field, pDEP (positive DEP) concentrates EVs at electrode edges (high-field regions), hydrogel layer separates electrodes from plasma
2. **Automated fluorescence quantification algorithm (MATLAB)**: Automatic identification of ROI (collection region) and BG (background region) based on electrode geometry, local noise subtraction (mean + 3σ), automated optical artifact removal
3. **Internal standard**: Known concentration of fluorescent NPs spiked into sample, corrects for chip-to-chip collection efficiency variation, co-collected and quantified with target biomarkers
4. **Optimization parameters**: AC voltage frequency/amplitude, flow rate, collection time, fluorescence exposure time, ROI/BG region definition thresholds, internal standard concentration
5. **Usable dynamic range**: Fluorescence intensity 1-2000 a.u., linear increase with exposure time and particle concentration

## Results
- Automated algorithm performed nearly identically to manual artifact removal (Pearson's r=0.999, 0.998, 36 patients, 2 biomarkers)
- Within usable dynamic range (1-2000 a.u.), fluorescence intensity linearly proportional to exposure time and particle concentration
- Internal standard reduced chip-to-chip collection efficiency variation, especially effective at low biomarker concentrations
- Internal standard maintained fluorescence intensity-exposure time linear trends, improved fluorescence intensity-particle concentration linear trends
- Biomarker quantification achievable in low SNR environments from early-stage cancer patient plasma
- DEP-based EV collection + automated fluorescence quantification demonstrated effective as a liquid biopsy platform

## Perspective
- Automated fluorescence quantification algorithm is applicable beyond DEP chips to any lab-on-a-chip with predictable collection regions
- Internal standard approach will become a standard tool for chip-to-chip and experiment-to-experiment variation correction
- Contributes to development of high-sensitivity liquid biopsy platforms for early cancer detection
- Multi-biomarker simultaneous quantification can improve cancer specificity and sensitivity
- Standardized validation protocols needed for clinical translation

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
