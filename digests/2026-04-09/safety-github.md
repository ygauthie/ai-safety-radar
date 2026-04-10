# GitHub Activity (2026-04-09)

## Key Discussions

Several important safety and alignment-related issues emerged across major repositories:

The [issue in anthropic-cookbook](https://github.com/anthropics/claude-cookbooks/issues/518) highlights a critical need for **automated verification gates** in the new Managed Agents architecture. While human-in-the-loop approval exists, there's no cookbook example showing how to automatically verify agent output before execution—a key safety consideration for autonomous systems.

Multiple pull requests focus on **evaluation robustness**. The [RAG guide fix](https://github.com/anthropics/claude-cookbooks/pull/521) addresses false positives in evaluation functions, while [HELM's summarization analyzer fix](https://github.com/stanford-crfm/helm/pull/4183) corrects a bug where relevance scores were incorrectly displayed under coherence metrics. Similarly, the [OpenAI cookbook's grade_completion fix](https://github.com/openai/openai-cookbook/pull/514) prevents false positives from case sensitivity and extra whitespace in evaluation functions.

The [LM Evaluation Harness fix for MMLU Pro](https://github.com/EleutherAI/lm-evaluation-harness/pull/3693) addresses a significant issue where fewshot reasoning was leaking into user roles under chat templates, potentially compromising evaluation integrity.

## Notable Releases

The Google DeepMind Gemma repository shows active development on **Gemma 4** with a [multiturn sampler implementation](https://github.com/google-deepmind/gemma/pull/612) and [README updates](https://github.com/google-deepmind/gemma/pull/619) documenting the new version.

TransformerLens continues expanding architecture support with adapters for [DeepSeek V3](https://github.com/TransformerLensOrg/TransformerLens/pull/1240), [Falcon](https://github.com/TransformerLensOrg/TransformerLens/pull/1241), and [CodeGen](https://github.com/TransformerLensOrg/TransformerLens/pull/1242), alongside a new [architecture relevancy testing system](https://github.com/TransformerLensOrg/TransformerLens/pull/1243) for prioritizing development efforts.

## Emerging Tools

Several new frameworks and patterns for AI safety practitioners emerged:

The [**self-improving agents cookbook**](https://github.com/anthropics/claude-cookbooks/pull/469) demonstrates a four-phase improvement cycle where agents execute, evaluate, analyze, and improve their responses across quality dimensions. This provides a structured approach to agent self-improvement with safety considerations.

New **Model Context Protocol (MCP)** implementations include both a [native Python MCP client cookbook](https://github.com/anthropics/claude-cookbooks/pull/499) and a [FastMCP primitives guide](https://github.com/anthropics/claude-cookbooks/pull/510), filling documentation gaps for developers wanting low-level control over MCP integrations.

The [**AI Portal multi-agent system**](https://github.com/anthropics/claude-cookbooks/pull/515) introduces comprehensive orchestration for autonomous browser automation with a Browser Hands Chrome extension, providing accessibility-first automation capabilities.

For evaluation, the LM Evaluation Harness added [**native Tensor Parallelism support**](https://github.com/EleutherAI/lm-evaluation-harness/pull/3692) for HuggingFace backends and [**TyDiQA Gold Passage tasks**](https://github.com/EleutherAI/lm-evaluation-harness/pull/3677) covering 11 languages with language-aware metrics.

The [**mathematical hallucination elimination cookbook**](https://github.com/openai/openai-cookbook/pull/2599) demonstrates routing computation to SymPy via tool use, providing a practical solution for reliable mathematical reasoning.