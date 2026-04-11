# GitHub Activity (2026-04-11)

## Key Discussions

Several important safety-related issues emerged from recent activity. Anthropic received a concerning [financial damage report](https://github.com/anthropics/claude-cookbooks/issues/489) where Claude Code agent errors cost a user ~$45 USD during a Kaggle competition, highlighting the real-world risks of autonomous agent systems. This parallels ongoing discussions about [output verification before agent actions](https://github.com/anthropics/claude-cookbooks/issues/518) in Anthropic's Managed Agents architecture, where developers are requesting automated verification gates to complement existing human-in-the-loop approval systems.

Multiple evaluation and grading systems showed reliability issues. The [LLM-based grading example](https://github.com/anthropics/claude-cookbooks/issues/497) in Anthropic's documentation contained string matching bugs causing false positives, while similar issues were found in [RAG evaluation functions](https://github.com/anthropics/claude-cookbooks/pull/521). EleutherAI's evaluation harness also had problems with [MMLU Pro fewshot answers leaking](https://github.com/EleutherAI/lm-evaluation-harness/pull/3693) into user roles under chat templates, potentially compromising evaluation integrity.

## Notable Releases

The evaluation ecosystem saw significant updates. EleutherAI's lm-evaluation-harness added support for [tool calls and reasoning tracking](https://github.com/EleutherAI/lm-evaluation-harness/pull/3685), enabling evaluation of model behavior when using tools or providing explanations. New multilingual capabilities arrived with [TyDiQA Gold Passage tasks](https://github.com/EleutherAI/lm-evaluation-harness/pull/3677) for 11 languages, expanding cross-lingual evaluation coverage.

OpenAI's cookbook introduced a practical approach to mathematical accuracy with [deterministic tool use via SymPy](https://github.com/openai/openai-cookbook/pull/2599), demonstrating how to eliminate LLM mathematical hallucinations by routing computation to external tools. The cookbook also added [secure text-to-SQL implementations](https://github.com/anthropics/claude-cookbooks/pull/495) showing defense-in-depth approaches against SQL injection and other attacks.

## Emerging Tools

Several new safety-focused tools and frameworks appeared. Anthropic expanded their [FastMCP primitives cookbook](https://github.com/anthropics/claude-cookbooks/pull/510) for building Model Control Protocol tools, while adding [multi-agent pipeline patterns](https://github.com/anthropics/claude-cookbooks/pull/517) with state handoffs and auto-retry mechanisms for more robust agent coordination.

TransformerLens continued expanding model architecture support with new adapters for [Qwen 3.5](https://github.com/TransformerLensOrg/TransformerLens/pull/1244), [Qwen3 MoE](https://github.com/TransformerLensOrg/TransformerLens/pull/1245), [CodeGen](https://github.com/TransformerLensOrg/TransformerLens/pull/1242), and [Falcon](https://github.com/TransformerLensOrg/TransformerLens/pull/1241) models, enabling mechanistic interpretability research across more diverse architectures. They also introduced [relevancy testing systems](https://github.com/TransformerLensOrg/TransformerLens/pull/1243) to prioritize architecture development based on model popularity and complexity metrics.

Aider enhanced its reflection capabilities by adding a [configurable max-reflections option](https://github.com/Aider-AI/aider/pull/5011), allowing users to adjust the number of self-correction attempts for complex coding tasks, while also adding support for [Kyma API models](https://github.com/Aider-AI/aider/pull/5019) through OpenAI-compatible endpoints.