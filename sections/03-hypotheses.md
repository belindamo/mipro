# Hypotheses

Primary Hypotheses:

Bootstrapping demonstrations hypothesis: Optimizing bootstrapped few-shot examples is essential for realizing greatest performance gains
Conditional rules hypothesis: Optimizing instructions becomes more essential for tasks with conditional rules that are (i) not immediately obvious to the LM and (ii) not expressible via limited few-shot examples
Joint optimization hypothesis: Optimizing both instructions and few-shot examples together leads to best results
Grounding hypothesis: Providing proposal LM with relevant context (data properties, program control flow, successful demonstrations) enables better instruction creation

Alternative Hypotheses:

Different credit assignment strategies (greedy, surrogate, history-based) will show varying effectiveness across different task types
Meta-optimization of proposal strategies will improve performance over fixed approaches

Predictions Based on Theory:

MIPRO will outperform baseline optimizers by effectively separating credit assignment from prompt proposal
Instruction optimization will show most impact on HotPotQA Conditional due to complex formatting rules
Grounding strategies will vary in effectiveness across different task types