# Research Concept & Direction

Research Problem and Objectives:
The main research question addresses how to optimize prompts for Language Model Programs (LM programs) - sophisticated pipelines of modular language model calls - to maximize downstream performance without access to module-level labels or gradients. The gap in knowledge being addressed is that existing prompt optimization work doesn't directly apply to multi-stage LM programs where individual module performance cannot be directly evaluated.
Research Goals:

Develop efficient prompt optimization strategies for arbitrary LM programs
Handle the "proposal challenge" (intractably large prompt space) and "credit assignment challenge" (jointly optimizing multiple distinct prompt variables)
Create optimizers that work under weak assumptions consistent with DSPy programming model abstractions

Scope and Expected Contributions:

Formalize the problem of prompt optimization for LM programs
Propose algorithmic design space with strategies for prompt proposal and credit assignment
Release benchmark suite for LM program optimizers spanning seven tasks
Develop MIPRO (Multi-prompt Instruction PRoposal Optimizer) that outperforms baselines