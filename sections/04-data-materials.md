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
