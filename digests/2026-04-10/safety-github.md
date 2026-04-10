# GitHub Activity (2026-04-10)

## Key Discussions

Several important AI safety discussions emerged from recent GitHub activity:

### Agent Architecture and Verification

Anthropic's cookbook repository saw significant focus on agent safety patterns. A new issue requests guidance on [output verification before agent actions](https://github.com/anthropics/claude-cookbooks/issues/518) in their Managed Agents architecture, highlighting the critical need for automated verification gates beyond human-in-the-loop approvals. This complements existing work on [self-improving agents with structured reflection](https://github.com/anthropics/claude-cookbooks/pull/469), which demonstrates a four-phase improvement cycle for agent self-evaluation across quality dimensions.

The repository also added a [multi-agent pipeline with state handoffs](https://github.com/anthropics/claude-cookbooks/pull/517), showing how to implement reliable agent coordination with auto-retry mechanisms - an important pattern for reducing failure modes in autonomous systems.

### Mathematical Reasoning Safety

OpenAI's cookbook introduced a practical approach to [eliminating mathematical hallucinations](https://github.com/openai/openai-cookbook/pull/2599) by routing computation to deterministic tools like SymPy rather than relying on LLM token prediction. This addresses a fundamental safety concern where models generate plausible-looking but incorrect mathematical results.

### Evaluation Framework Issues

The LM Evaluation Harness saw important fixes for evaluation integrity:
- A [critical bug in median aggregation](https://github.com/EleutherAI/lm-evaluation-harness/pull/3668) that returned incorrect results for unsorted inputs
- [Preprocessing corruption in GPQA tasks](https://github.com/EleutherAI/lm-evaluation-harness/pull/3691) where regex patterns stripped legitimate scientific notation from answer choices
- [Few-shot evaluation errors in MMLU Pro](https://github.com/EleutherAI/lm-evaluation-harness/pull/3693) where reasoning was incorrectly included in user turns under chat templates

These fixes highlight how subtle bugs in evaluation frameworks can compromise safety assessments of AI systems.

## Emerging Tools

### Model Control Protocol Integration

Anthropic's cookbook expanded MCP (Model Control Protocol) support with both a [native Python MCP client](https://github.com/anthropics/claude-cookbooks/pull/499) and [FastMCP primitives guide](https://github.com/anthropics/claude-cookbooks/pull/510). These tools enable more structured and verifiable tool use patterns, important for maintaining control over AI system capabilities.

### Browser Automation with Safety Controls

A new [AI Portal multi-agent system](https://github.com/anthropics/claude-cookbooks/pull/515) introduces a Browser Hands Chrome extension for accessibility-first automation. This represents an important development in maintaining human oversight over autonomous web interactions.

### Tensor Parallelism for Evaluation

The LM Evaluation Harness added [native tensor parallelism support](https://github.com/EleutherAI/lm-evaluation-harness/pull/3692) for Hugging Face models, enabling more efficient evaluation of large models - crucial for comprehensive safety testing at scale.

## Notable Releases

### Model Updates

Both Anthropic and OpenAI repositories updated their model references:
- Anthropic's [courses repository migrated](https://github.com/anthropics/courses/pull/152) from deprecated Claude 3 model IDs to current Claude 4 versions across 36 course files
- Google DeepMind updated their [Gemma README to include Gemma 4](https://github.com/google-deepmind/gemma/pull/619)

### TransformerLens Architecture Expansion

TransformerLens made significant progress supporting new architectures with safety research implications:
- [DeepSeek v3 adapter](https://github.com/TransformerLensOrg/TransformerLens/pull/1240) with MLA attention handling
- [Falcon architecture support](https://github.com/TransformerLensOrg/TransformerLens/pull/1241) with ALiBi implementation
- [CodeGen architecture adapter](https://github.com/TransformerLensOrg/TransformerLens/pull/1242)

These additions expand the toolkit available for mechanistic interpretability research across diverse model architectures.

### Security Updates

Aider addressed several security vulnerabilities with dependency updates:
- [aiohttp 3.13.3 → 3.13.4](https://github.com/Aider-AI/aider/pull/5015) (CVE-2026-22815)
- [litellm 1.82.3 → 1.83.0](https://github.com/Aider-AI/aider/pull/5016) (CVE-2026-35029)  
- [pygments 2.19.2 → 2.20.0](https://github.com/Aider-AI/aider/pull/5017) (CVE-2026-4539)
- [requests 2.32.5 → 2.33.0](https://github.com/Aider-AI/aider/pull/5018) (CVE-2026-25645)