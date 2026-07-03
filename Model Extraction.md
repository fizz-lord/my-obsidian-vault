---
type: research-note
status: open
severity: high
topic: model-extraction
created: 2026-07-03
tags: [model-extraction, red-teaming, api]
---

# Model Extraction

**Tags:** `#model-extraction #red-teaming`

## Overview
Model extraction aims to replicate a proprietary model using API queries.

## Techniques
- Fidelity extraction via large query sets.
- Architecture reverse engineering.
- Membership inference attacks.

## Related Topics
- [[AI Red Teaming]]
- [[Adversarial Examples]]

## Workflow: Extraction Test
Input: API endpoint and budget.
Output: replica fidelity score and evidence.

Steps:
1. Enumerate API behavior patterns.
2. Generate comparative query set.
3. Log outputs and compute similarity metrics.
4. Store results in vault.

## Backlinks
- [[AI Red Teaming]]
- [[AI Security Index]]
