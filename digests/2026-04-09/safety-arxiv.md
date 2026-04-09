# ArXiv - AI Safety Papers (2026-04-09)

## Key Papers

### [TraceSafe: A Systematic Assessment of LLM Guardrails on Multi-Step Tool-Calling Trajectories](https://arxiv.org/abs/2604.07223v1)
This paper introduces TraceSafe-Bench, the first comprehensive benchmark for evaluating safety guardrails during multi-step AI agent execution rather than just final outputs. As LLMs evolve into autonomous agents, the vulnerability surface shifts from static responses to dynamic execution traces, making this work crucial for understanding how safety mechanisms perform in real-world agentic scenarios.

### [AgentCity: Constitutional Governance for Autonomous Agent Economies via Separation of Power](https://arxiv.org/abs/2604.07007v1)
Addresses the "Logic Monopoly" problem where autonomous AI agents operating across organizational boundaries create opaque collective behavior that no single human can govern. The paper proposes a constitutional framework with separation of powers to ensure democratic oversight of agent societies, representing a significant contribution to AI governance at scale.

### [How to sketch a learning algorithm](https://arxiv.org/abs/2604.07328v1)
Presents a novel data deletion scheme that can predict how AI models would behave if certain training data had been excluded. This work has major implications for AI safety, privacy, and interpretability by enabling efficient analysis of training data influence without full model retraining.

### [CSA-Graphs: A Privacy-Preserving Structural Dataset for Child Sexual Abuse Research](https://arxiv.org/abs/2604.07132v1)
Introduces a privacy-preserving approach to CSAI detection research by providing structural graph representations instead of raw images. This addresses the critical challenge of advancing AI safety in sensitive domains while maintaining strict ethical and legal compliance.

### [Designing Safe and Accountable GenAI as a Learning Companion with Women Banned from Formal Education](https://arxiv.org/abs/2604.07253v1)
Examines the unique safety and privacy requirements for GenAI systems supporting women's education in restrictive and surveilled contexts. This research highlights critical considerations for AI deployment in high-risk environments where user safety depends on system design choices.

### [Personalized RewardBench: Evaluating Reward Models with Human Aligned Personalization](https://arxiv.org/abs/2604.07343v1)
Introduces the first benchmark specifically designed to assess reward models' ability to capture individual user preferences rather than general response quality. This work is essential for pluralistic AI alignment, addressing how well reward models can accommodate diverse human values and preferences.

### [A comparative analysis of machine learning models in SHAP analysis](https://arxiv.org/abs/2604.07258v1)
Provides systematic analysis of SHAP (SHapley Additive exPlanations) performance across different ML models, addressing the critical need for explainable AI in high-stakes applications. Understanding when and how SHAP explanations remain reliable is crucial for safe AI deployment.

### [Information as Structural Alignment: A Dynamical Theory of Continual Learning](https://arxiv.org/abs/2604.07108v1)
Proposes the Informational Buildup Framework (IBF) as an alternative to traditional approaches for continual learning that avoid catastrophic forgetting. Rather than adding external mechanisms, this approach derives retention from learning dynamics themselves, offering a more principled foundation for safe, adaptive AI systems.

## Trends

**Multi-Step Safety Assessment**: The emergence of benchmarks like TraceSafe-Bench reflects growing recognition that AI safety evaluation must extend beyond static outputs to dynamic execution trajectories, especially as LLMs become autonomous agents.

**Governance at Scale**: Research on constitutional frameworks for AI agent societies (AgentCity) indicates increasing focus on systematic governance mechanisms for multi-agent AI systems operating without centralized oversight.

**Privacy-Preserving Research Methods**: The development of structural datasets (CSA-Graphs) and data deletion schemes demonstrates growing sophistication in enabling AI safety research while maintaining privacy and ethical constraints.

**Contextual Safety Design**: Work on GenAI for education in restrictive contexts highlights the need for safety frameworks that account for specific deployment environments and user vulnerabilities.

**Interpretability Beyond Explanation**: Research is moving beyond simple explainability toward understanding fundamental mechanisms of learning, retention, and decision-making in AI systems, as seen in work on continual learning dynamics and reward model personalization.

**Robustness Under Real-World Conditions**: Multiple papers address challenges like temporal distribution shift, partial observability, and noisy data, indicating maturation from idealized benchmarks toward practical deployment considerations.