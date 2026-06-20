# Self-driving laboratories to autonomously navigate the protein fitness landscape

## Citation (NLM)
Rapp JT, Bremer BJ, Romero PA. Self-driving laboratories to autonomously navigate the protein fitness landscape. Nat Chem Eng. 2024;1:97-107. doi: 10.1038/s44286-023-00002-4

**DOI:** [https://doi.org/10.1038/s44286-023-00002-4](https://doi.org/10.1038/s44286-023-00002-4)

---

## Background
- Protein engineering has nearly limitless applications across chemistry, energy, and medicine, but creating new proteins with improved or novel functions remains slow, labor-intensive, and inefficient
- The human hypothesis-experiment-interpretation cycle is highly inefficient and can take years
- Robot scientists and self-driving laboratories combine automated learning, reasoning, and experimentation to accelerate scientific discovery
- Biological phenotypes are complex and nonlinear, genomic search spaces are high-dimensional, making autonomous protein engineering particularly challenging
- Existing automated workflows require some human input and are not fully autonomous

## Key Experiment Methods
1. **SAMPLE platform**: Self-driving Autonomous Machines for Protein Landscape Exploration - intelligent agent learns protein sequence-function relationships and designs new proteins
2. **Bayesian optimization (BO) agent**: Gaussian process (GP) model to understand fitness landscape, balancing exploration and exploitation
3. **Multi-output GP model**: Simultaneously predicts active/inactive classification and continuous property (thermostability)
4. **UCB positive / Expected UCB algorithms**: Sampling informed by activity probability (Pactive) to avoid inactive 'holes'
5. **Fully automated experimental pipeline**: Golden Gate cloning (gene assembly) → PCR → T7-based cell-free protein expression → colorimetric/fluorescent assays (T50 thermostability)
6. **Exception handling and data quality control**: dsDNA EvaGreen verification, reaction curve fitting, background activity checks

## Results
- Four independent SAMPLE agents deployed to optimize glycoside hydrolase thermostability
- All agents converged on enzymes at least 12°C more stable than starting sequences
- Discovered optimized proteins while searching less than 2% of the full landscape
- Automated pipeline achieved T50 measurement reproducibility within 1.6°C error
- Total 9h from gene assembly (1h) → PCR (1h) → expression (3h) → thermostability assay (3h) per design-to-data point
- UCB positive / Expected UCB methods found optimal sequences with 3-4x fewer samples than standard UCB (26 measurements in simulation)

## Perspective
- Self-driving laboratories can implement fully autonomous design-test-learn cycles in protein engineering
- Integration of Bayesian optimization and automated experimentation dramatically improves protein optimization efficiency
- SAMPLE platform is a general-purpose protein engineering tool applicable across biological engineering and synthetic biology
- Experimental measurement noise affects agent search behavior but convergence remains robust
- Future expansion to multi-objective optimization, larger sequence spaces, and complex functional properties is possible

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
