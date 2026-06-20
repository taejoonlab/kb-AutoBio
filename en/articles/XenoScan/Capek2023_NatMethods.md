# EmbryoNet: using deep learning to link embryonic phenotypes to signaling pathways

## Citation (NLM)
Čapek D, Safroshkin M, Morales-Navarrete H, Toulany N, Arutyunov G, Kurzbach A, Bihler J, Hagauer J, Kick S, Jones F, Jordan B, Müller P. EmbryoNet: using deep learning to link embryonic phenotypes to signaling pathways. Nat Methods. 2023;20:815-823. doi: 10.1038/s41592-023-01873-4

**DOI:** [https://doi.org/10.1038/s41592-023-01873-4](https://doi.org/10.1038/s41592-023-01873-4)

---

## Background
- Early embryogenesis is orchestrated by seven major signaling pathways (BMP, RA, Wnt, FGF, Nodal, Shh, PCP), and loss of function leads to characteristic developmental defects
- Phenotypic defect classification can identify underlying signaling mechanisms but relies on expert knowledge and lacks standardized classification schemes
- Automated, high-throughput quantitative phenotyping platform for zebrafish developmental images is needed

## Key Experiment Methods
1. **EmbryoNet deep learning model**: ResNet-based convolutional neural network (CNN) for automated classification of zebrafish signaling mutants, trained on over 2 million images
2. **Time-dependent developmental trajectory model**: Multi-timestamp input architecture accounting for stage-specific phenotypic changes during development
3. **Seven signaling pathway classification**: Unbiased identification of BMP, RA, Wnt, FGF, Nodal, Shh, and PCP loss-of-function mutants
4. **High-throughput drug screening application**: EmbryoNet applied to high-throughput drug screens to resolve mechanism of action (MOA) of pharmaceutical substances
5. **Optimization parameters**: CNN layer configuration (7×7, 3×3, 1×1 ConvRelu), residual blocks, global average pooling, timestamp channel count, training dataset size

## Results
- EmbryoNet accurately classified zebrafish mutants for all seven major signaling pathways
- Combined with time-dependent developmental trajectory model for high-precision identification and classification of phenotypic defects
- Robustly identified signaling defects in evolutionarily distant species
- Resolved mechanism of action of pharmaceutical substances in high-throughput drug screens
- Released over 2 million training/testing images to the community

## Perspective
- Deep learning-based automated phenotyping is broadly applicable to developmental biology and signaling pathway research
- Integration with high-throughput drug screening accelerates MOA elucidation in drug discovery
- Standardized classification schemes overcome limitations of expert-dependent phenotypic evaluation
- Future expansion to multi-species and multi-stage universal phenotyping framework
- Publicly available large-scale image dataset serves as foundational infrastructure for developmental deep learning research

---

*Processed by **Qwen3.6 Plus** (opencode-go) on 2026-06-20*
