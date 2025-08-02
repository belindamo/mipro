# Literature Review

Existing Research:

Prompt Optimization: Recent work includes gradient-guided search (Shin et al., 2020), reranking brute force search (Gao et al., 2021), evolutionary algorithms (Fernando et al., 2023), prompting other LMs (Yang et al., 2023; Zhou et al., 2023), and reinforcement learning approaches (Deng et al., 2022; Zhang et al., 2022)
Language Model Programs: Sophisticated prompting techniques and chaining for multi-stage pipelines (Wei et al., 2022; Chen et al., 2022; Wu et al., 2022; Khattab et al., 2022)
DSPy Framework: Khattab et al. (2024) present a programming model for expressing LM programs and optimizing prompts/weights, but only explore bootstrapping-based optimizers

Gaps in Literature:

Majority of existing prompt optimization work doesn't apply to multi-stage LM programs lacking gold labels for individual calls
Current optimizers cannot tune instructions for multi-prompt pipelines
Limited work on joint optimization of instructions and demonstrations across multiple modules

Methodologies Used:

APE (Zhou et al., 2023), OPRO (Yang et al., 2024), EvoPrompt (Guo et al., 2024) for single-stage optimization
Sordoni et al. (2023) explore joint prompt optimization for stacked LLM calls using variational inference but requires log probabilities