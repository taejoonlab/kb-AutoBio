# Unbiased identification of cell identity in dense mixed neural cultures

## Citation (NLM)
De Beuckeleer S, Van De Looverbosch T, Van Den Daele J, Ponsaerts P, De Vos WH. Unbiased identification of cell identity in dense mixed neural cultures. eLife. 2025;13:RP95273. doi: 10.7554/eLife.95273

**DOI:** [https://doi.org/10.7554/eLife.95273](https://doi.org/10.7554/eLife.95273)

---

## Background
- iPSC technology enables generation of brain-resident cell types (neurons, astrocytes, microglia, etc.), but iPSC line-to-line variability and lack of comprehensive cell type characterization technology hinder preclinical screening adoption
- Quantitative and systematic characterization of cell type composition in dense, mixed neural cultures is needed
- Conventional cell type identification based on population-level time in culture classification is inaccurate
- Morphological single-cell profiling can quantify cell composition in complex mixed neural cultures

## Key Experiment Methods
1. **Cell painting-based imaging assay**: Multi-fluorescent staining visualizes morphological features (nucleus, cytoplasm, actin, mitochondria, etc.), high-content microscopy for image acquisition
2. **CNN-based cell type classification**: Convolutional neural network recognizes cell types from cell painting images, benchmarked with neuroblastoma/astrocytoma pure and mixed cultures
3. **Regionally restricted cell profiling**: Nuclear ROI + surrounding environment achieves classification accuracy equivalent to whole-cell images, maintains prediction accuracy even in dense cultures
4. **Iterative data erosion**: Stepwise reduction of input image regions to identify minimum required ROI, demonstrating that nucleus + surrounding is sufficient for classification
5. **Application to iPSC-derived neural cultures**: Differentiation status assessment (mature neurons vs neural progenitor ratio), microglia clearly distinguished from neurons regardless of reactivity state, tiered strategy for activated vs non-activated state classification
6. **Optimization parameters**: ROI definition (nuclear + surrounding vs whole cell), CNN architecture, classification thresholds, cell painting staining combinations, image resolution

## Results
- Cell painting + CNN classification accuracy >96% (neuroblastoma/astrocytoma pure/mixed cultures)
- Regionally restricted profiling (nuclear ROI + surrounding) achieved equivalent accuracy to whole-cell images, maintained in semi-confluent and very dense cultures
- Cell-based prediction outperformed population-level time-based classification in iPSC-derived neural cultures (96% vs 86%)
- Microglia clearly distinguished from neurons in mixed iPSC-derived neural cultures, regardless of reactivity state
- Tiered strategy enabled additional classification of activated vs non-activated microglia (lower accuracy but identifiable)
- Morphological single-cell profiling demonstrated effective for quantifying cell composition in complex mixed neural cultures

## Perspective
- Cell painting + CNN contributes as a fast, inexpensive assay for iPSC-derived cell culture quality control
- Regionally restricted profiling is applicable even in dense cultures, suitable for real-world preclinical screening environments
- Single-cell level analysis contributes to batch-to-batch and line-to-line variability monitoring
- Future expansion to multi-cell type simultaneous classification, disease model validation, and drug screening quality control
- Integration with automated imaging enables high-throughput characterization of iPSC-based neurological disease models

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
