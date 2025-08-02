# Data & Materials

Datasets:

HotPotQA: Multi-hop QA requiring reasoning over multiple Wikipedia articles (500 train, 500 dev, 2000 test)
HotPotQA Conditional: Modified version with conditional formatting rules based on answer type (500 train, 200 dev, 200 test)
Iris: Classic flower classification dataset (75 train, 75 test)
Iris-Typo: Same as Iris but with intentional misspelling in prompt
Heart Disease: Binary classification for heart disease prediction (120 train, 183 test)
ScoNe: Natural language inference with logical reasoning and negation (500 train, 500 dev, 1200 test)
HoVer: Multi-hop claim verification over Wikipedia (500 train, 500 dev, 1520 test)

Models:

Task Model: Llama3-8B (primary LM used in programs)
Proposer Model: GPT-3.5 (default for instruction generation), GPT-4o (for challenging tasks)
Bootstrap Teacher Model: Llama-3-8B (default), GPT-4o (for ScoNe and HoVer)

Statistics:

Time span: Training datasets of 500 examples, optimization budgets of 20-50 full evaluation trials
Dataset size: Total ~8,000 examples across 7 tasks
Coordinates: Tasks span classification, QA, retrieval, and logical reasoning

Experiments
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