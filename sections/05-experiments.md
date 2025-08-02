# Experiments

Experimental Design:

Three optimization categories:

Instructions-only optimization
Few-shot demonstrations-only optimization
Joint instruction & demonstration optimization


Optimizer Methods Tested:

Bootstrap Random Search (baseline)
Module-Level OPRO
0-Shot MIPRO
0-Shot MIPRO++
Bayesian Bootstrap
MIPRO (full joint optimization)



Control and Treatment Conditions:

Control: Un-optimized LM Program baseline
Ablation Studies: Module-Level OPRO with/without Grounding
Treatment Variations: Different combinations of instruction proposal and credit assignment strategies

Methodology:

5 runs per method on each task for statistical robustness
Wilcoxon signed-rank tests for significance testing
Mini-batch evaluation (size B) for efficient exploration
Tree Structured Parzen Estimator for Bayesian optimization

Validity Measures:

Statistical significance testing between methods
Cross-validation across diverse task types
Evaluation on held-out test sets
Comparison against strong DSPy baseline optimizers