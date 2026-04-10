# ArXiv - AI Safety Papers (2026-04-09)

## Key Papers

### [TraceSafe: A Systematic Assessment of LLM Guardrails on Multi-Step Tool-Calling Trajectories](https://arxiv.org/abs/2604.07223v1)
This paper introduces TraceSafe-Bench, the first comprehensive benchmark for evaluating safety guardrails during multi-step tool-use trajectories rather than just final outputs. This addresses a critical gap as LLMs evolve from chatbots to autonomous agents, where intermediate execution steps may pose the primary vulnerability surface.

### [AgentCity: Constitutional Governance for Autonomous Agent Economies via Separation of Power](https://arxiv.org/abs/2604.07007v1)
Proposes a governance framework for autonomous AI agent societies operating across organizational boundaries, addressing the "Logic Monopoly" problem where no single human can audit emergent multi-agent behavior. The framework implements separation of powers to enable oversight and accountability in agent economies.

### [How to sketch a learning algorithm](https://arxiv.org/abs/2604.07328v1)
Presents a novel data deletion scheme that can predict how deep learning models would behave if certain training data had been excluded, with applications to interpretability, privacy, and understanding data influence. This addresses the fundamental question of how training data choices affect AI model behavior.

### [Designing Safe and Accountable GenAI as a Learning Companion with Women Banned from Formal Education](https://arxiv.org/abs/2604.07253v1)
Examines the design requirements for safe generative AI systems in surveilled, gender-restrictive contexts where formal education access is limited. This research highlights critical considerations for AI safety in high-risk deployment scenarios involving vulnerable populations.

### [CSA-Graphs: A Privacy-Preserving Structural Dataset for Child Sexual Abuse Research](https://arxiv.org/abs/2604.07132v1)
Introduces a privacy-preserving structural dataset for child sexual abuse imagery classification research, replacing explicit visual content with structural representations. This enables reproducible research while maintaining strict ethical and legal compliance.

### [A comparative analysis of machine learning models in SHAP analysis](https://arxiv.org/abs/2604.07258v1)
Analyzes the effectiveness of SHAP (SHapley Additive exPlanations) across different machine learning models, contributing to explainable AI methods that are crucial for trustworthy deployment in high-stakes situations.

### [Personalized RewardBench: Evaluating Reward Models with Human Aligned Personalization](https://arxiv.org/abs/2604.07343v1)
Introduces a benchmark for evaluating how well reward models capture individual user preferences rather than just general response quality. This addresses the critical challenge of pluralistic alignment in LLMs that need to accommodate diverse human values.

### [EmoMAS: Emotion-Aware Multi-Agent System for High-Stakes Edge-Deployable Negotiation with Bayesian Orchestration](https://arxiv.org/abs/2604.07003v1)
Proposes a Bayesian multi-agent framework that transforms emotional decision-making from reactive to strategic in high-stakes negotiation scenarios, addressing the computational and privacy limitations of large language models in edge deployment settings.

## Trends

**Safety Evaluation Beyond Final Outputs**: There's a notable shift toward evaluating AI safety during intermediate processes rather than just final outputs, as seen in trajectory-based safety assessment and multi-step tool-use evaluation.

**Governance for Multi-Agent Systems**: Growing recognition that autonomous agent societies require constitutional frameworks and governance mechanisms to ensure accountability and prevent emergent risks from uncontrolled agent interactions.

**Privacy-Preserving AI Research**: Increased focus on developing methodologies that enable sensitive AI research (such as abuse detection) while maintaining privacy and ethical compliance through structural representations and data abstraction.

**Contextual and Cultural AI Safety**: Emerging attention to AI safety in specific cultural and political contexts, particularly for vulnerable populations in surveilled or restrictive environments.

**Personalized Alignment**: Movement beyond one-size-fits-all AI alignment toward systems that can accommodate diverse individual preferences while maintaining safety constraints.

**Edge-Deployable Safety**: Focus on developing safety mechanisms that work under computational and connectivity constraints, particularly relevant for mobile and embedded AI systems.

**Explainable AI Integration**: Continued development of interpretability methods as fundamental components of AI safety, with emphasis on model-agnostic approaches that can provide insights across different architectures.