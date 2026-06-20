# Cluster learning-assisted directed evolution

## Citation (NLM)
Qiu Z, Wu R, Wang Y, Wei G. Cluster learning-assisted directed evolution. Nat Comput Sci. 2021;1:815-825. doi: 10.1038/s43588-021-00168-y

**DOI:** [https://doi.org/10.1038/s43588-021-00168-y](https://doi.org/10.1038/s43588-021-00168-y)

---

## Background
- Directed evolution (DE) improves protein properties by mimicking natural selection, but fitness evaluation is costly and time-consuming
- Fitness landscape is a high-dimensional surface mapping amino acid sequences to activity, selectivity, stability, etc.; epistasis limits greedy search to local optima
- Multi-site-saturation mutagenesis creates combinatorial libraries that overwhelm screening capacity
- ML-assisted directed evolution (MLDE) uses active learning with surrogate model + acquisition function
- CLADE (Cluster Learning-Assisted Directed Evolution) framework: unsupervised clustering for training set preselection, fitness heterogeneity identification

## Key Experiment Methods
1. **Unsupervised clustering strategy**: Self-supervised protein embedding (variational autoencoder, transformer, etc.) for sequence feature extraction, clustering to partition fitness-heterogeneous subspaces
2. **Training set preselection**: Representative sequences selected from each cluster, supervised model trained on small informative subset - minimized experimental burden (2 iterations)
3. **Zero-shot predictor utilization**: Unsupervised predictor for fitness prediction without experiments, constraining training set selection
4. **Surrogate model + greedy search**: Trained model for virtual fitness landscape navigation, greedy search for protein fitness optimization
5. **CLADE framework validation**: Applied to diverse systems including enzyme evolution (activity/selectivity improvement), fluorescent proteins, protein stability optimization
6. **Optimization parameters**: clustering algorithm selection, number of clusters, embedding model, training set size, acquisition function, iteration count

## Results
- Unsupervised clustering successfully identified fitness heterogeneity, with clear fitness distribution differentiation between clusters
- Supervised model trained on small informative subset (fraction of full library), minimizing experimental burden to 2 iterations
- CLADE achieved state-of-the-art results compared to existing MLDE, discovering higher fitness variants with same number of experiments
- Effective navigation of epistatic landscapes, overcoming greedy search local optima problem
- Generalization performance confirmed across diverse protein systems (enzymes, fluorescent proteins, stability optimization)
- Self-supervised embedding captured latent biological information from vast unlabeled sequence data, transferred to downstream tasks

## Perspective
- Integration of unsupervised clustering + supervised learning dramatically improves MLDE efficiency
- Self-supervised protein embedding is established as a core tool in protein engineering
- CLADE framework efficiently discovers high-fitness variants while minimizing experimental burden
- Future expansion to multi-objective optimization (activity + stability + selectivity) and metabolic pathway optimization
- Integration with automated DE platforms enables self-driving protein engineering

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
