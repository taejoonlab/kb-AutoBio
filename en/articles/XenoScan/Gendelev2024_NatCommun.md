# Deep phenotypic profiling of neuroactive drugs in larval zebrafish

## Citation (NLM)
Gendelev L, Taylor J, Myers-Turnbull D, Chen S, McCarroll MN, Arkin MR, Kokel D, Keiser MJ. Deep phenotypic profiling of neuroactive drugs in larval zebrafish. Nat Commun. 2024;15:9955. doi: 10.1038/s41467-024-54375-y

**DOI:** [https://doi.org/10.1038/s41467-024-54375-y](https://doi.org/10.1038/s41467-024-54375-y)

---

## Background
- CNS drug mechanisms of action remain poorly understood due to GPCR/ion channel pathway complexity and polypharmacology
- Phenotypic screening circumvents single-target limitations by prioritizing complex biological readouts
- Larval zebrafish enable high-throughput small molecule screening format for discovering neuroactive molecules relevant to mammalian physiology
- Traditional correlation distance-based phenotypic distance computation fails to distinguish subtle phenotypes and suffers from shortcut learning

## Key Experiment Methods
1. **High-throughput zebrafish behavioral screening**: 650 CNS-active compounds screened in high replicate in 96-well plates, behavioral responses recorded under light/acoustic stimuli
2. **Motion Index (MI) time series**: Bulk motion measured from video frames, traditionally computed using correlation distance for phenotypic distance
3. **Deep metric learning model**: Trained on zebrafish behavioral profiles, well-wise physical randomization implemented to eliminate shortcut learning artifacts
4. **Prospective in vitro validation**: Radio-ligand binding assays against human protein targets validated model predictions (58% hit rate)
5. **Optimization parameters**: well randomization strategy, MI time series processing, metric learning architecture, correlation distance vs learned distance comparison

## Results
- Deep metric learning model substantially outperformed correlation distance in phenotypic distance computation
- Well-wise randomization resolved initial model's shortcut learning (exploiting subtle experimental artifacts)
- Generalization confirmed on orthogonal dataset of diverse drug-like compounds
- Prospective in vitro validation achieved 58% hit rate, crossing species and chemical scaffold boundaries
- Zebrafish phenotypic screening combined with metric learning demonstrated robust scaffold hopping capabilities

## Perspective
- Deep metric learning will become a standard tool for high-throughput phenotypic screening data analysis
- Well randomization is critical for preventing shortcut learning in phenotypic screening
- Zebrafish behavioral screening has broad applications in CNS drug discovery and target deconvolution
- Future integration of multi-stimulus and multi-timescale data will improve phenotypic resolution
- Cross-species translatability validation accelerates preclinical drug discovery pipelines

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
