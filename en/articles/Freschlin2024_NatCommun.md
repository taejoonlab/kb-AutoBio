# Neural network extrapolation to distant regions of the protein fitness landscape

## Citation (NLM)
Freschlin CR, Fahlberg SA, Heinzelman P, Romero PA. Neural network extrapolation to distant regions of the protein fitness landscape. Nat Commun. 2024;15:6405. doi: 10.1038/s41467-024-50712-3

**DOI:** [https://doi.org/10.1038/s41467-024-50712-3](https://doi.org/10.1038/s41467-024-50712-3)

---

## Background
- ML has transformed protein engineering by constructing models of sequence-function relationships to accelerate discovery of new biomolecules
- ML-guided protein design requires models trained on local sequence-function data to accurately predict distant fitness peaks
- Neural networks' capacity to extrapolate beyond training data needs evaluation
- Model-guided design using protein G (GB1)-IgG binding data, with experimental testing of thousands of GB1 variants for systematic extrapolation evaluation

## Key Experiment Methods
1. **Neural network architecture panel**: Linear models, MLP, CNN, transformer, etc. trained on same data, comparing landscape inference and inductive biases of each architecture
2. **Model-guided in silico search**: ML models explore sequence-function landscape, thousands of GB1 variants designed (sampling vast sequence space outside training regime)
3. **High-throughput yeast display assay**: Experimental validation of thousands of designed GB1 variants, IgG binding function measurement, comparison of model predictions with experimental results
4. **Extrapolation evaluation**: Local extrapolation (near training data) vs distant extrapolation (deep into sequence space) performance comparison
5. **Ensemble approach**: CNN simple ensemble achieves robust design, integrating individual model design preferences
6. **Optimization parameters**: model architecture selection, training data size, number of mutations, sequence positions, amino acid substitution types, ensemble composition

## Results
- Each model architecture inferred markedly different landscapes from the same data, producing unique design preferences
- Simpler models (linear, shallow MLP) excelled at local extrapolation - successfully designed high-fitness proteins
- Sophisticated CNNs could venture deep into sequence space but designed proteins that fold yet lose function
- CNN simple ensemble enabled robust design of high-performing variants in the local landscape
- Model inductive biases influenced learning of different aspects of the protein fitness landscape
- First systematic benchmark of ML model predictive power with experimental validation

## Perspective
- Model architecture selection has decisive impact on design strategy in protein engineering
- Ensemble approaches compensate for single model limitations, improving protein engineering robustness
- Distant extrapolation remains challenging - gap between model predictions and experimental validation needs resolution
- Future integration with active learning for continuous model improvement with experimental data in closed-loop
- ML-guided protein design has broad applications in enzyme, antibody, and therapeutic protein development

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
