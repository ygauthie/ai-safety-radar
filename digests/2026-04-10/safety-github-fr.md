# GitHub Activity (2026-04-10)

## Discussions Clés

L'activité GitHub révèle plusieurs développements importants concernant la sécurité et l'alignement de l'IA :

**Vérification et Contrôle des Agents**
Une [discussion sur les agents gérés d'Anthropic](https://github.com/anthropics/claude-cookbooks/issues/518) propose l'ajout d'exemples de vérification automatique des sorties d'agents avant l'exécution d'actions. Cette approche complète les systèmes d'approbation humaine existants par des garde-fous automatisés, abordant un défi critique de sécurité dans les systèmes d'agents autonomes.

**Nouvelles Architectures d'Agents**
Plusieurs nouvelles contributions démontrent des patterns d'agents avancés : un [système d'agents auto-améliorants avec réflexion structurée](https://github.com/anthropics/claude-cookbooks/pull/469) qui implémente un cycle d'amélioration en quatre phases, et des [pipelines multi-agents avec transferts d'état](https://github.com/anthropics/claude-cookbooks/pull/517) montrant l'orchestration planificateur-travailleur-vérificateur.

**Élimination des Hallucinations Mathématiques**
Un [nouveau notebook OpenAI](https://github.com/openai/openai-cookbook/pull/2599) démontre comment éliminer les hallucinations mathématiques des LLM en acheminant les calculs vers SymPy via l'utilisation d'outils, offrant une solution pratique à un problème de sécurité bien connu.

## Nouveaux Outils

**Intégration MCP Native**
Anthropic a ajouté des guides pour l'[utilisation native du SDK Python MCP](https://github.com/anthropics/claude-cookbooks/pull/499) et les [primitives FastMCP](https://github.com/anthropics/claude-cookbooks/pull/510), facilitant l'intégration d'outils externes avec Claude tout en maintenant un contrôle approprié.

**Parallélisme Tensoriel pour l'Évaluation**
Le LM Evaluation Harness a introduit le [support natif du parallélisme tensoriel pour le backend HF](https://github.com/EleutherAI/lm-evaluation-harness/pull/3692), permettant une évaluation accélérée des modèles distribués via `torchrun`.

**Système d'Évaluation TyDiQA**
L'ajout de [tâches TyDiQA Gold Passage](https://github.com/EleutherAI/lm-evaluation-harness/pull/3677) fournit une évaluation QA extractive multilingue pour 11 langues avec des métriques F1 et de correspondance exacte conscientes de la langue.

## Corrections Critiques

**Corrections d'Évaluation GPQA**
Une [correction importante](https://github.com/EleutherAI/lm-evaluation-harness/pull/3691) retire la regex qui supprimait le contenu entre crochets des choix de réponses GPQA, qui corrompait la nomenclature chimique et les notations de physique légitimes.

**Améliorations de Sécurité des Dépendances**
Plusieurs projets ont mis à jour des dépendances avec des CVE connus : Aider a mis à jour [requests](https://github.com/Aider-AI/aider/pull/5018), [pygments](https://github.com/Aider-AI/aider/pull/5017), [litellm](https://github.com/Aider-AI/aider/pull/5016), et [aiohttp](https://github.com/Aider-AI/aider/pull/5015), tandis qu'OpenAI a mis à jour [node-forge](https://github.com/openai/openai-cookbook/pull/2597).

**Expansion d'Architecture**
TransformerLens continue d'étendre la prise en charge des architectures avec de nouveaux adaptateurs pour [DeepSeek v3](https://github.com/TransformerLensOrg/TransformerLens/pull/1240), [Falcon](https://github.com/TransformerLensOrg/TransformerLens/pull/1241), et [CodeGen](https://github.com/TransformerLensOrg/TransformerLens/pull/1242), améliorant la capacité de recherche en interprétabilité sur diverses architectures de modèles.