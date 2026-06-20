# An autonomous laboratory for the accelerated synthesis of novel materials

## Citation (NLM)
Szymanski NJ, Rendy B, Fei Y, Kumar RE, He T, Milsted D, McDermott MJ, Gallant M, Cubuk ED, Merchant A, Kim H, Jain A, Bartel CJ, Persson K, Zeng Y, Ceder G. An autonomous laboratory for the accelerated synthesis of novel materials. Nature. 2023;624:86-93. doi: 10.1038/s41586-023-06734-w

**DOI:** [https://doi.org/10.1038/s41586-023-06734-w](https://doi.org/10.1038/s41586-023-06734-w)

---

## Background
- Advances in computational materials science have enabled large-scale ab initio screening for new materials, but experimental validation remains slow and labor-intensive
- Autonomous experimental platforms are needed: agents that can interpret data and make decisions based on it
- Prior autonomous lab efforts were limited to specific domains such as carbon nanotube yield, photovoltaic performance, and photocatalysis
- Solid-state inorganic powder synthesis presents unique challenges compared to liquid handling, including milling and diverse physical properties

## Key Experiment Methods
1. **A-Lab platform**: Three integrated stations (powder dispensing/mixing, heating with 4 box furnaces, XRD characterization) connected by robotic arms
2. **Synthesis recipe generation**: ML model trained on literature data proposes initial recipes by analogy to known materials; second ML model suggests synthesis temperature
3. **ARROWS3 active learning**: When recipes fail, integrates ab initio reaction energies with observed outcomes to predict solid-state reaction pathways and iteratively optimize
4. **XRD pattern analysis**: Probabilistic ML models for phase identification, confirmed by automated Rietveld refinement; target phase yield (>50%) assessed
5. **Target selection**: 58 novel compounds on or near (<10 meV/atom) the convex hull from Materials Project and Google DeepMind; filtered for air stability

## Results
- Successfully synthesized 41 of 58 target compounds over 17 days of continuous operation (71% success rate)
- Spanned 33 elements and 41 structural prototypes (oxides, phosphates, etc.)
- Literature-based ML recipes succeeded on first attempt for most; failures improved via ARROWS3 active learning
- Analysis of 17 failures revealed actionable insights for computational screening and synthesis design
- Demonstrated capability to synthesize some metastable compounds

## Perspective
- AI-driven autonomous laboratories can bridge the gap between computational prediction and experimental validation
- Integration of ab initio computation, ML algorithms, literature knowledge, and robotics is key to accelerating materials discovery
- Failure analysis reveals limitations in computational screening (metastability prediction, reaction kinetics) and points to improvements
- Future expansion to liquid handling, thin-film synthesis, and electrochemical evaluation is possible
- Need to establish collaboration paradigms between human researchers and autonomous systems

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
