# Robotic search for optimal cell culture in regenerative medicine

## Citation (NLM)
Kanda GN, Tsuzuki T, Terada M, Sakai N, Motozawa N, Masuda T, Nishida M, Watanabe CT, Higashi T, Horiguchi SA, Kudo T, Kamei M, Sunagawa GA, Matsukuma K, Sakurada T, Ozawa Y, Takahashi M, Takahashi K, Natsume T. Robotic search for optimal cell culture in regenerative medicine. eLife. 2022;11:e77007. doi: 10.7554/eLife.77007

**DOI:** [https://doi.org/10.7554/eLife.77007](https://doi.org/10.7554/eLife.77007)

---

## Background
- Induced differentiation in regenerative medicine is highly experience- and skill-dependent, often taking years to establish optimal conditions
- Cell culture outcomes are greatly affected by chemical stimuli (reagent type, dose, timing) and physical manipulation (pipetting strength, vibration, CO2 incubator handling)
- Existing automated cell culture machines use fixed-process automation, limiting flexible parameter exploration
- Robotic arms can repeatedly perform identical operations with high precision, maintain constant physical parameters, and log errors

## Key Experiment Methods
1. **LabDroid system**: Versatile humanoid robot executing cell culture protocols, with integrated microscope for AI-based image processing and cell quality assessment
2. **iPSC-RPE differentiation protocol digitization**: Five steps - seeding, preconditioning, passage, RPE differentiation (induction), RPE maintenance culture
3. **Batch Bayesian Optimization (BBO)**: Explores optimal conditions among 200 million parameter combinations, processing 8 × 6-well plates simultaneously (48 wells/batch)
4. **Automated operations**: Three programmed task types - seeding, medium exchange type I (with reagent preparation), medium exchange type II, and passage
5. **Quality assessment**: Pigmentation score used as objective function, automated microscope image analysis

## Results
- Explored 143 conditions over 111 days, achieving 88% improvement in iPSC-RPE production compared to manual optimization (by pigmentation score)
- Robot-produced iPSC-RPE cells met regenerative medicine research application criteria
- BBO algorithm efficiently explored experimental space, reducing time compared to manual optimization
- High reproducibility and error logging of robotic operations ensured experimental transparency

## Perspective
- Autonomous robotic AI systems can dramatically accelerate cell culture condition optimization
- Applicable beyond regenerative medicine to drug screening, tissue engineering, and other fields
- Combination of robotization and AI optimization presents a new paradigm for laboratory automation
- Future expansion to multi-objective optimization (pigmentation + morphology + gene expression) is possible
- Versatile robots like LabDroid can flexibly adapt to changing research protocols

---

*Processed by **opencode** (opencode-go) on 2026-06-20*
