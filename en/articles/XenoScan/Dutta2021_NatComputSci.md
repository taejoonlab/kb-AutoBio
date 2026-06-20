# Machine learning-guided directed evolution of enzymes

## Citation (NLM)
Dutta A, et al. Cluster learning-assisted directed evolution. Nat Comput Sci. 2021;1:815-825. doi: 10.1038/s43588-021-00110-2

**DOI:** [https://doi.org/10.1038/s43588-021-00110-2](https://doi.org/10.1038/s43588-021-00110-2)

---

## Background
- Directed evolution is central to enzyme engineering, but fitness landscape exploration is experimentally costly and time-consuming
- ML learns sequence-function relationships to reduce search space and efficiently predict active variants
- Clustering-based learning identifies fitness heterogeneity and preselects informative training sets
- Self-driving lab concepts are applied to automate the entire enzyme optimization process

## Key Experiment Methods
1. **ML-guided directed evolution**: Surrogate model trained on sequence-function data, acquisition function determines next experiment priorities
2. **Clustering-assisted training**: Unsupervised clustering partitions fitness landscape, representative sequence selection minimizes experimental burden
3. **Zero-shot predictor**: Unsupervised model predicts fitness without experiments, constrains training set selection
4. **Greedy search optimization**: Trained model navigates virtual landscape, approaches global optimum with minimal experiments
5. **Optimization parameters**: model architecture, clustering algorithm, training set size, acquisition function, iteration count

## Results
- ML-guided directed evolution dramatically reduced experiment counts compared to conventional DE while maintaining or improving fitness
- Clustering-assisted training effectively identified fitness heterogeneity, model trained on small informative subset
- Zero-shot predictor pre-screened promising variants without experiments
- Enzyme activity, stability, and selectivity optimized with minimal experiment iterations
- Self-driving lab concept successfully applied to enzyme engineering pipelines

## Perspective
- ML + directed evolution integration dramatically improves throughput and speed of enzyme engineering
- Clustering-based learning streamlines high-dimensional fitness landscape exploration
- Self-driving enzyme engineering platforms have broad applications in industrial biotechnology and pharmaceutical production
- Future expansion to multi-objective optimization, metabolic pathway optimization, and new-to-nature reaction design
- Automated DE platforms are evolving as core infrastructure for synthetic biology

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
