---
type: research-note
status: open
severity: high
topic: jailbreak
created: 2026-07-03
tags: [jailbreak, prompt-injection, llm-security, attack-surface]
---

# Emoji Jailbreaks via Token Segmentation Bias

## Overview
Embedding emojis inside prompts can shift token boundaries and embeddings enough for malicious requests to bypass safety filters and Judge LLM's.

## Mechanism
- Tokenizers split words around emojis, e.g. `sens😎itive` becomes separate tokens.
- Segmented token embeddings differ from the original word embedding.
- Small embedding shifts allow harmful content to move out of the classifier danger zone.

## Impact
- Bypasses safety filters and judge LLM moderation.
- Enables generation of hate speech, disinformation, and harmful instructions.
- Can also be used to extract training data from models.

## Defences
- Emoji aware tokenizers that preserve semantic token boundaries.
- Embedding space robustness via adversarial training with emoji perturbations.
- Context aware safety filters that reason over the full prompt, not keywords.
- Judge LLMs trained on emoji jailbreak examples.
- Human in the loop review for suspicious or novel prompting patterns.

## Source
- Based on Google Cloud Community analysis of emoji jailbreak research.

## Related
- [[Jailbreak Techniques]]
- [[Prompt Injection]]
- [[AI Red Teaming]]
- [[AI Security Index]]
