# Results & Analysis

Key Findings - Five Lessons:
Lesson 1: Optimizing bootstrapped demonstrations is key to achieving best performance

Bootstrap Random Search beats best instruction-only optimizer in 6/7 tasks
High variation in performance from different few-shot sets indicates importance of selection

Lesson 2: Joint optimization with MIPRO yields best overall performance

MIPRO statistically significantly outperforms second-best optimizer on 4/7 tasks
Exceptions: HotPotQA, Heart Disease, and Iris (without typo) where instructions less valuable

Lesson 3: Instruction optimization most important for conditional rules

HotPotQA Conditional: 0-shot instruction optimization outperforms demonstration-only
Iris-Typo: Instruction optimizer corrects mistakes in seed prompt
Effect strongest when rules are (i) not obvious to LM and (ii) not expressible via few examples

Lesson 4: Grounding helps instruction proposal but strategy varies by task

Essential for HotPotQA and HoVer performance improvements
Hurts performance on ScoNe, motivating adaptive approaches like MIPRO++
Learned importance scores reveal dataset summary crucial for ScoNe, less important for HotPotQA/HoVer

Lesson 5: More to learn about LM program optimizers

Mixed results comparing Module-Level OPRO, 0-Shot MIPRO, and 0-Shot MIPRO++
Bayesian Bootstrap outperforms Bootstrap Random Search for ScoNe but not statistically significant elsewhere
Future work needed on optimization dynamics across different budget scenarios

Performance Results:

MIPRO achieves up to 13% accuracy improvement over baselines
Best performance on 5/7 tasks when jointly optimizing instructions and demonstrations
Significant improvements on ScoNe (79.4% vs baseline 57.0%), HotPotQA Conditional (23.3% vs 10.5%), and others

Statistical Significance:

Wilcoxon signed-rank tests confirm significance (p < .05) for top performers
Results averaged across 5 runs for robustness
Bold values in results table indicate statistically significant best performance